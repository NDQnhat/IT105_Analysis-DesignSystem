### 1. **Planning (Lập kế hoạch)**
- Xác định mục tiêu dự án: xây dựng ứng dụng giúp giảng viên điểm danh nhanh, chính xác, lưu trữ dữ liệu tập trung.  
- Phân tích phạm vi, nguồn lực, ngân sách và thời gian.  
- Lên kế hoạch nhân sự (quản lý dự án, lập trình viên, tester...).  
- Xác định rủi ro và cách giảm thiểu (mạng yếu, dữ liệu sai, lỗi đồng bộ...).  

---

### 2. **Analysis (Phân tích yêu cầu)**
- Thu thập và phân tích yêu cầu từ người dùng (giảng viên, sinh viên, phòng đào tạo).  
- Xác định các chức năng chính: điểm danh theo lớp, xem lịch sử, báo cáo chuyên cần, đồng bộ dữ liệu.  
- Mô tả yêu cầu phi chức năng: bảo mật, tốc độ xử lý, dễ sử dụng.  
- Xây dựng tài liệu đặc tả yêu cầu phần mềm (SRS).  

---

### 3. **Design (Thiết kế hệ thống)**
- Thiết kế kiến trúc hệ thống (mobile app + server + database).  
- Thiết kế giao diện người dùng (UI/UX): màn hình đăng nhập, danh sách lớp, điểm danh.  
- Thiết kế cơ sở dữ liệu: bảng SinhVien, LopHoc, DiemDanh, GiangVien.  
- Thiết kế API kết nối giữa client và server.  

---

### 4. **Implementation (Lập trình/triển khai)**
- Tiến hành lập trình ứng dụng mobile (Android/iOS).  
- Xây dựng backend (API, cơ sở dữ liệu).  
- Viết mã theo chuẩn, kiểm soát phiên bản bằng Git.  
- Tích hợp các chức năng: điểm danh bằng mã QR, cập nhật trạng thái, đồng bộ dữ liệu thời gian thực.  

---

### 5. **Testing (Kiểm thử)**
- Kiểm thử chức năng: điểm danh, đăng nhập, xem báo cáo.  
- Kiểm thử giao diện: tính dễ dùng, hiển thị đúng thông tin.  
- Kiểm thử bảo mật: đăng nhập, phân quyền người dùng.  
- Kiểm thử hiệu năng: tải nhanh, ổn định khi nhiều người dùng cùng lúc.  
- Sửa lỗi (bug) và tinh chỉnh trước khi triển khai chính thức.  

---

### 6. **Deployment & Maintenance (Triển khai và Bảo trì)**
- Triển khai ứng dụng lên server và kho ứng dụng (Google Play, App Store).  
- Hướng dẫn người dùng (giảng viên, sinh viên).  
- Theo dõi hiệu suất, phản hồi người dùng và cập nhật định kỳ.  
- Bảo trì, nâng cấp chức năng mới (ví dụ: điểm danh bằng khuôn mặt, xuất báo cáo tự động).  