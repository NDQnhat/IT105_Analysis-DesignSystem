1. Yếu tố con người (Người dùng & tổ chức)

| **Thành phần**                       | **Tác động đến yêu cầu kỹ thuật**                                                                                                                                  |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Bác sĩ, y tá, kỹ thuật viên**      | Hệ thống phải có giao diện trực quan, thao tác nhanh, hiển thị thông tin bệnh nhân rõ ràng, hỗ trợ tìm kiếm hồ sơ nhanh chóng.                                     |
| **Nhân viên hành chính, lễ tân**     | Cần chức năng đăng ký khám, quản lý lịch hẹn và thanh toán dễ dùng; yêu cầu phân quyền rõ ràng theo vị trí.                                                        |
| **Bệnh nhân (hoặc người nhà)**       | Cần cổng thông tin bệnh nhân / app di động giúp xem lịch hẹn, kết quả khám, thanh toán online → yêu cầu kỹ thuật về giao diện thân thiện, bảo mật dữ liệu cá nhân. |
| **Ban giám đốc / quản lý bệnh viện** | Yêu cầu hệ thống có khả năng tổng hợp dữ liệu, báo cáo thống kê, biểu đồ, dashboard quản lý.                                                                       |


2. Quy trình nghiệp vụ y tế (Business Processes)

| **Thành phần**                   | **Tác động đến yêu cầu kỹ thuật**                                                                          |
| -------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| **Quy trình khám – chữa bệnh**   | Hệ thống phải hỗ trợ quy trình nhiều bước (đăng ký → khám → xét nghiệm → chẩn đoán → kê toa → thanh toán). |
| **Quản lý thuốc và vật tư y tế** | Cần module quản lý kho, cảnh báo hết hàng, tích hợp mã vạch / QR code.                                     |
| **Hồ sơ bệnh án điện tử (EMR)**  | Đòi hỏi hệ thống lưu trữ an toàn, dễ truy xuất, tuân thủ tiêu chuẩn dữ liệu y tế (ví dụ HL7, FHIR).        |


3. Cơ sở hạ tầng kỹ thuật (Hardware & Network)

| **Thành phần**                          | **Tác động đến yêu cầu kỹ thuật**                                                          |
| --------------------------------------- | ------------------------------------------------------------------------------------------ |
| **Máy tính, thiết bị đầu cuối**         | Ứng dụng cần tương thích với nhiều thiết bị (máy tính, máy in phiếu, máy xét nghiệm).      |
| **Mạng nội bộ và Internet**             | Phải đảm bảo hiệu năng và khả năng làm việc offline tạm thời khi mất kết nối.              |
| **Máy chủ (Server) và lưu trữ dữ liệu** | Cần yêu cầu cao về bảo mật, sao lưu định kỳ, khả năng mở rộng khi số lượng bệnh nhân tăng. |


4. Quy định pháp lý và tiêu chuẩn y tế

| **Thành phần**                                                | **Tác động đến yêu cầu kỹ thuật**                                                                      |
| ------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ |
| **Luật bảo vệ dữ liệu cá nhân (VD: Nghị định 13/2023/NĐ-CP)** | Phải mã hóa thông tin bệnh nhân, quản lý truy cập theo vai trò, có cơ chế ghi log truy vết.            |
| **Quy định Bộ Y tế về hồ sơ bệnh án điện tử**                 | Hệ thống phải đáp ứng định dạng chuẩn, khả năng ký số và lưu trữ lâu dài.                              |
| **Chuẩn an toàn thông tin (ISO 27001, HIPAA)**                | Ảnh hưởng đến yêu cầu bảo mật, xác thực đa yếu tố, và truyền dữ liệu qua kết nối an toàn (HTTPS, VPN). |


5. Hệ thống bên ngoài (External Systems)

| **Thành phần**                           | **Tác động đến yêu cầu kỹ thuật**                                                                  |
| ---------------------------------------- | -------------------------------------------------------------------------------------------------- |
| **Hệ thống bảo hiểm y tế**               | Cần tích hợp API để tra cứu, xác nhận quyền lợi, và gửi dữ liệu thanh toán.                        |
| **Phòng xét nghiệm, chẩn đoán hình ảnh** | Hệ thống phải kết nối với thiết bị chuyên dụng (máy X-quang, máy siêu âm) để nhận kết quả tự động. |
| **Ngân hàng / Cổng thanh toán**          | Yêu cầu tích hợp thanh toán trực tuyến, tuân thủ chuẩn bảo mật PCI DSS.                            |


6. Yếu tố môi trường vật lý và vận hành

| **Thành phần**                                   | **Tác động đến yêu cầu kỹ thuật**                                                                                |
| ------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------- |
| **Điều kiện mạng và điện tại bệnh viện**         | Cần cơ chế lưu tạm dữ liệu offline, đồng bộ lại khi có kết nối.                                                  |
| **Khối lượng người dùng lớn trong giờ cao điểm** | Hệ thống phải được thiết kế hiệu năng cao, hỗ trợ truy cập đồng thời, có khả năng cân bằng tải (load balancing). |

