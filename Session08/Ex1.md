### Phân tích và chú thích:

![Ex1](/Session08/assets/Ex1.png)


### Mô tả và đề xuất cải tiến:

* Ảnh gốc: Giao diện hiển thị danh sách 4 tin bất động sản nổi bật, mỗi tin gồm hình ảnh, tiêu đề, vị trí, giá, diện tích và nút “Xem chi tiết”.

* Ảnh chú thích lỗi UI: 
- Nút “Xem chi tiết” quá nhỏ, khó bấm trên thiết bị di động.
- Nhãn “Tin nổi bật” màu vàng không nổi bật so với nền ảnh.
- Khoảng cách giữa các tin không đều, gây cảm giác chật chội.

* Nhận xét tổng quan
Giao diện đơn giản, dễ hiểu nhưng thiếu sự tinh chỉnh về bố cục và hành vi tương tác. Người dùng có thể cảm thấy khó thao tác, đặc biệt trên thiết bị di động.

* Phân tích lỗi UI/UX
1. Bố cục
- Khoảng cách giữa các tin: Không đều, thiếu khoảng trắng khiến giao diện bị nghẹt thở.
- Kích thước nút "Xem chi tiết": Quá nhỏ, dễ bị bỏ qua hoặc khó bấm.
- Vị trí nhãn "Tin nổi bật": Nằm trên ảnh, màu vàng không đủ tương phản, dễ bị chìm.

2. Màu sắc
- Màu nhãn “Tin nổi bật”: Vàng trên nền ảnh nhiều chi tiết gây khó đọc.
- Thiếu hệ màu nhất quán: Không có màu chủ đạo rõ ràng, gây cảm giác rời rạc.

3. Hành vi
- Nút không có trạng thái phản hồi: Không có hiệu ứng hover hoặc nhấn, gây nghi ngờ về tính năng.
- Thiếu menu lọc hoặc phân loại: Người dùng không thể dễ dàng tìm loại bất động sản mong muốn.

4. UX
- Không có thông tin bổ sung khi hover: Thiếu mô tả ngắn hoặc thông tin nổi bật.
- Không có phân loại rõ ràng: Nhà phố, biệt thự, căn hộ… hiển thị lẫn lộn.
- Giá hiển thị không thống nhất đơn vị: Có tin dùng “triệu”, có tin dùng “tỷ”, dễ gây nhầm lẫn.

* Nguyên nhân tiềm ẩn:
- Thiết kế chưa tối ưu cho thiết bị di động: Kích thước nút và khoảng cách chưa phù hợp.
- Thiếu quy chuẩn thiết kế UI: Không có hệ thống màu, lưới bố cục hoặc hành vi tương tác rõ ràng.
- Không có kiểm thử người dùng: Giao diện có thể chưa được kiểm tra thực tế với người dùng thật.

* Đề xuất cải tiến:

| Vấn đề                       | Giải pháp đề xuất                                     | 
| ---------------------------- | ----------------------------------------------------- |
| Nút “Xem chi tiết” nhỏ       | Tăng kích thước, thêm hiệu ứng hover và nhấn          | 
| Nhãn “Tin nổi bật” không nổi | Đổi màu sang cam hoặc đỏ, thêm viền trắng hoặc nền mờ | 
| Khoảng cách chật chội        | Tăng padding giữa các tin, dùng lưới bố cục rõ ràng   | 


