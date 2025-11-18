### UI sơ bộ cho chức năng "Làm bài Quiz"


![UI](/Session10/assets/Ex2_UI.png)

### Thiết kế bảng cơ sở dữ liệu cho Use Case "Làm bài Quiz"

1. Bảng: quizzes – Thông tin chung về quiz


| Tên cột         | Kiểu dữ liệu | Mô tả                    | Ghi chú                |
| --------------- | ------------ | ------------------------ | ---------------------- |
| quiz_id         | INT          | ID quiz                  | PK                     |
| course_id       | INT          | Khóa học liên quan       | FK → courses.course_id |
| title           | VARCHAR(255) | Tên quiz                 |                        |
| time_limit      | INT          | Thời gian làm bài (phút) |                        |
| total_questions | INT          | Tổng số câu              |                        |


2. Bảng: quiz_questions – Danh sách câu hỏi trong quiz


| Tên cột       | Kiểu dữ liệu | Mô tả             | Ghi chú              |
| ------------- | ------------ | ----------------- | -------------------- |
| question_id   | INT          | ID câu hỏi        | PK                   |
| quiz_id       | INT          | Thuộc quiz nào    | FK → quizzes.quiz_id |
| question_text | TEXT         | Nội dung câu hỏi  |                      |
| order_number  | INT          | Số thứ tự câu hỏi |                      |


3. Bảng: quiz_answers – Các đáp án của mỗi câu hỏi


| Tên cột     | Kiểu dữ liệu | Mô tả                 | Ghi chú                         |
| ----------- | ------------ | --------------------- | ------------------------------- |
| answer_id   | INT          | ID đáp án             | PK                              |
| question_id | INT          | Thuộc câu hỏi nào     | FK → quiz_questions.question_id |
| answer_text | TEXT         | Nội dung đáp án       |                                 |
| is_correct  | BOOLEAN      | Đáp án đúng hay không |                                 |


4. Bảng: quiz_attempts – Lưu bài làm của sinh viên


| Tên cột    | Kiểu dữ liệu | Mô tả             | Ghi chú            |
| ---------- | ------------ | ----------------- | ------------------ |
| attempt_id | INT          | ID bài làm        | PK                 |
| user_id    | INT          | Người làm bài     | FK → users.user_id |
| quiz_id    | INT          | Quiz đã làm       | FK                 |
| start_time | DATETIME     | Thời gian bắt đầu |                    |
| end_time   | DATETIME     | Thời gian nộp     |                    |
| score      | FLOAT        | Điểm cuối cùng    |                    |


5. Bảng: quiz_attempt_answers – Lưu câu trả lời của người dùng


| Tên cột            | Kiểu dữ liệu | Mô tả                     | Ghi chú                       |
| ------------------ | ------------ | ------------------------- | ----------------------------- |
| attempt_answer_id  | INT          | ID dòng                   | PK                            |
| attempt_id         | INT          | Thuộc bài làm nào         | FK → quiz_attempts.attempt_id |
| question_id        | INT          | Câu hỏi tương ứng         | FK                            |
| selected_answer_id | INT          | Đáp án mà người dùng chọn | FK → quiz_answers.answer_id   |
| is_correct         | BOOLEAN      | Tự động tính sau khi nộp  |                               |


