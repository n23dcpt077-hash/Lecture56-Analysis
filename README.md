# 💻 Lecture 5–6: Requirements Analysis  
**Trường:** Học viện Công nghệ Bưu chính Viễn thông (PTIT)  
**Môn học:** Nhập môn Công nghệ Phần mềm  
**Sinh viên thực hiện:** Nguyễn Thị Ngọc Hân – N23DCPT077  

---

## 📘 I. Giới thiệu
Tài liệu và bài tập chương 6 – **Phân tích yêu cầu phần mềm (Requirements Analysis)**,  
bao gồm lý thuyết, câu hỏi củng cố và các bài tập thực hành UML.

**Nội dung chính:**
- Phần lý thuyết: trắc nghiệm, câu hỏi ngắn, thảo luận nhóm, tình huống  
- Phần thực hành: sơ đồ UML, bài Java OOP, test case, cơ sở dữ liệu 3NF  

---

## 🧩 II. Liên kết tệp và hình ảnh

### 📄 File tổng hợp bài làm
👉 [Tải xuống file Word tại đây](https://github.com/n23dcpt077-hash/Lecture56-Analysis/blob/main/N23DCPT077_LECTURE6_ANALYSIS.docx)

---

### 🧱 1️⃣ Class Diagram – Library Management
![Class Diagram](https://github.com/n23dcpt077-hash/Lecture56-Analysis/blob/main/classdiagram.png?raw=true)

---

### 🔁 2️⃣ Sequence Diagram – Login Process
![Sequence Diagram](https://github.com/n23dcpt077-hash/Lecture56-Analysis/blob/main/sequence.png?raw=true)

---

### 🏥 3️⃣ ERD – Hospital Management
![ERD Diagram](https://github.com/n23dcpt077-hash/Lecture56-Analysis/blob/main/ERDdiagram.png?raw=true)

---

## 🧮 III. Bài tập thực hành (Practice Section)

### 🔹 1. Java OOP – Quản lý sinh viên
**Mục tiêu:** Áp dụng lập trình hướng đối tượng để tạo chương trình quản lý sinh viên (Student Management).  
**Cấu trúc lớp:**
- `Student`: chứa thông tin sinh viên  
- `Course`: chứa thông tin môn học  
- `Enrollment`: quan hệ giữa sinh viên và môn học  

📘 *Mỗi lớp được định nghĩa với thuộc tính riêng và phương thức truy xuất dữ liệu (getter/setter).*

---

### 🔹 2. UML Class Diagram – Library Management
**Mục tiêu:** Thiết kế sơ đồ lớp cho hệ thống quản lý thư viện.  
Các lớp chính: `Book`, `Member`, `Loan`, `Librarian`, `Reservation`, `Catalog`.  
Quan hệ giữa các lớp: 1–nhiều, kế thừa, và kết hợp (composition).

---

### 🔹 3. Test Case – Đăng ký tài khoản
**Mục tiêu:** Viết test case cho chức năng đăng ký tài khoản trên website.  
**Ví dụ test case:**
| STT | Mô tả kiểm thử | Input | Kết quả mong đợi |
|-----|----------------|--------|------------------|
| 1 | Đăng ký tài khoản hợp lệ | Email, mật khẩu hợp lệ | Hiển thị thông báo thành công |
| 2 | Thiếu email | Không nhập email | Báo lỗi yêu cầu nhập email |

---

### 🔹 4. Database Design – Bán hàng trực tuyến (3NF)
**Mục tiêu:** Thiết kế CSDL cho hệ thống e-Commerce và chuẩn hóa đến 3NF.  
**Các bảng chính:** `Product`, `Customer`, `Order`, `OrderDetail`, `Payment`.  
**Đảm bảo:** không trùng lặp dữ liệu, có khóa chính/ngoại rõ ràng.

---

### 🔹 5. Java Code – Nguyên tắc đóng gói (Encapsulation)
**Ví dụ:**
```java
public class Account {
  private double balance;

  public void deposit(double amount) {
    if (amount > 0) balance += amount;
  }

  public double getBalance() {
    return balance;
  }
}
````

---

### 🔹 6. Sequence Diagram – Đăng nhập hệ thống

**Mục tiêu:** Mô tả trình tự trao đổi thông điệp giữa các đối tượng trong chức năng Login.
Đối tượng: `User`, `LoginUI`, `AuthController`, `Database`.
👉 [Xem hình Sequence Diagram ở trên](#-2️⃣-sequence-diagram--login-process)

---

### 🔹 7. Unit Test – Tính tổng hai số

**Mục tiêu:** Viết chương trình kiểm thử đơn vị (JUnit).
**Ví dụ:**

```java
@Test
public void testSum() {
  assertEquals(5, Calculator.sum(2, 3));
}
```

---

### 🔹 8. Test Scenario – Thanh toán (E-Commerce)

**Mục tiêu:** Viết kịch bản kiểm thử chức năng thanh toán.
**Các bước chính:**

1. Người dùng chọn sản phẩm
2. Kiểm tra giỏ hàng
3. Nhập thông tin thanh toán
4. Nhấn “Xác nhận” → hiển thị thông báo thành công

---

### 🔹 9. ERD – Quản lý bệnh viện

**Mục tiêu:** Biểu diễn quan hệ giữa các thực thể: `Patient`, `Doctor`, `Treatment`, `Prescription`, `Bill`, ...
👉 [Xem hình ERD ở trên](#-3️⃣-erd--hospital-management)

---

### 🔹 10. Use Case – Hệ thống đặt vé máy bay

**Mục tiêu:** Mô tả use case “Đặt vé thành công / Hết chỗ”.
Bao gồm Actor: `Khách hàng`, `Hệ thống`, `Nhân viên`.
Tình huống chính & ngoại lệ: đặt vé, thanh toán, thông báo hết chỗ.

---

## 🧭 IV. Cấu trúc thư mục

```
📦 Lecture56-Analysis
 ┣ 📜 README.md
 ┣ 📜 N23DCPT077_LECTURE6_ANALYSIS.docx
 ┣ 🖼️ classdiagram.png
 ┣ 🖼️ sequence.png
 ┗ 🖼️ ERDdiagram.png
```

---

## ⚙️ V. Công cụ sử dụng

* **PlantUML Web Editor** → vẽ và xuất sơ đồ UML
* **Visual Studio Code / IntelliJ IDEA** → viết Java
* **GitHub** → lưu trữ, chia sẻ và quản lý version

---

## ✨ VI. Thông tin nộp bài

* **Họ và tên:** Nguyễn Thị Ngọc Hân
* **Mã số sinh viên:** N23DCPT077
* **Lớp:** D23CQPT01-N
* **Giảng viên hướng dẫn:** ThS. Châu Văn Vân
* **Thời gian hoàn thành:** Tháng 10 / 2025

---

📍 **Liên kết repo chính thức:**
🔗 [https://github.com/n23dcpt077-hash/Lecture56-Analysis](https://github.com/n23dcpt077-hash/Lecture56-Analysis)


