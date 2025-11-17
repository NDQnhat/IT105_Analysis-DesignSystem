1. Thực thể: User


| **Entity** | **Attribute** | **Kiểu dữ liệu** | **Vai trò**                                 |
| ---------- | ------------- | ---------------- | ------------------------------------------- |
| User       | UserID (PK)   | INT              | Định danh duy nhất cho người dùng.          |
| User       | FullName      | VARCHAR(100)     | Lưu tên đầy đủ của người dùng.              |
| User       | Email         | VARCHAR(100)     | Dùng để đăng nhập và liên hệ.               |
| User       | Role          | VARCHAR(20)      | Phân loại người dùng: Student / Instructor. |


2. Thực thể: Course


| **Entity** | **Attribute** | **Kiểu dữ liệu** | **Vai trò**                      |
| ---------- | ------------- | ---------------- | -------------------------------- |
| Course     | CourseID (PK) | INT              | Định danh duy nhất của khóa học. |
| Course     | CourseName    | VARCHAR(150)     | Tên khóa học.                    |
| Course     | Description   | TEXT             | Mô tả nội dung khóa học.         |
| Course     | CreatedDate   | DATE             | Ngày tạo khóa học.               |


3. Thực thể: Enrollment


| **Entity** | **Attribute**     | **Kiểu dữ liệu** | **Vai trò**                              |
| ---------- | ----------------- | ---------------- | ---------------------------------------- |
| Enrollment | EnrollmentID (PK) | INT              | Định danh duy nhất cho lượt đăng ký học. |
| Enrollment | UserID (FK)       | INT              | Tham chiếu đến người dùng đăng ký học.   |
| Enrollment | CourseID (FK)     | INT              | Tham chiếu đến khóa học tương ứng.       |
| Enrollment | EnrollDate        | DATE             | Ngày người dùng đăng ký khóa học.        |
