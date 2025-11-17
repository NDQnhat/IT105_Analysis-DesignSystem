### Bảng thể hiện mối quan hệ giữa các thực thể:


| Tình huống                  | Thực thể liên quan  | Kiểu quan hệ | Giải thích                                                                          |
| --------------------------- | ------------------- | ------------ | ----------------------------------------------------------------------------------- |
| 1. Sinh viên – Mã sinh viên | Student – StudentID | **1 – 1**    | Mỗi sinh viên có đúng một mã duy nhất, và mỗi mã chỉ thuộc về một sinh viên.        |
| 2. Khách hàng – Đơn hàng    | Customer – Order    | **1 – N**    | Một khách hàng có thể đặt nhiều đơn hàng; nhưng mỗi đơn hàng chỉ có 1 khách hàng.   |
| 3. Sinh viên – Môn học      | Student – Course    | **N – N**    | Một sinh viên học nhiều môn; mỗi môn cũng có nhiều sinh viên → Cần bảng trung gian. |
