1. Chuẩn hóa về 1NF:

Yêu cầu của 1NF:
- Không có thuộc tính đa trị (multi-value).
- Mỗi ô chỉ chứa một giá trị nguyên tử.
=> Tách nhiều sản phẩm thành nhiều dòng.

#### Bảng: Order (sau 1NF):

| OrderID (PK) | CustomerName | Phone      | Product | Total  |
| ------------ | ------------ | ---------- | ------- | ------ |
| HD001        | An           | 0912345678 | Bút bi  | 50,000 |
| HD001        | An           | 0912345678 | Vở      | 50,000 |
| HD001        | An           | 0912345678 | Thước   | 50,000 |
| HD002        | Bình         | 0987654321 | Sách    | 80,000 |
| HD002        | Bình         | 0987654321 | Bút chì | 80,000 |

2. Chuẩn hóa về 2NF:

Yêu cầu của 2NF:
- Đã thỏa 1NF.
- Không có phụ thuộc bộ phận vào khóa chính.
=> Bảng 1NF có khóa chính là (OrderID, Product).
Các thuộc tính CustomerName, Phone, Total không phụ thuộc vào Product, chỉ phụ thuộc vào OrderID ⇒ vi phạm 2NF.
=> Giải pháp: Tách thành 2 bảng

#### Bảng: Orders (thỏa 2NF):

| OrderID (PK) | CustomerName | Phone      | Total  |
| ------------ | ------------ | ---------- | ------ |
| HD001        | An           | 0912345678 | 50,000 |
| HD002        | Bình         | 0987654321 | 80,000 |


#### Bảng: OrderDetails (thỏa 2NF):

| OrderID (FK) | Product (PK) |
| ------------ | ------------ |
| HD001        | Bút bi       |
| HD001        | Vở           |
| HD001        | Thước        |
| HD002        | Sách         |
| HD002        | Bút chì      |


3. Chuẩn hóa về 3NF

Yêu cầu của 3NF:
- Đã thỏa 2NF.
- Không có phụ thuộc bắc cầu (transitive dependency)
Trong bảng Orders:

- CustomerName → Phone
→ Một khách hàng có thể xuất hiện nhiều lần ⇒ nên tách khách hàng ra bảng riêng.

=> Tách bảng Customer


#### Bảng: Customers (thỏa 3NF):

| CustomerID (PK) | CustomerName | Phone      |
| --------------- | ------------ | ---------- |
| C001            | An           | 0912345678 |
| C002            | Bình         | 0987654321 |


#### Bảng: Orders (thỏa 3NF):

| OrderID (PK) | CustomerID (FK) | Total  |
| ------------ | --------------- | ------ |
| HD001        | C001            | 50,000 |
| HD002        | C002            | 80,000 |


#### Bảng: OrderDetails (thỏa 3NF):

| OrderDetailID (PK) | OrderID (FK) | Product |
| ------------------ | ------------ | ------- |
| OD001              | HD001        | Bút bi  |
| OD002              | HD001        | Vở      |
| OD003              | HD001        | Thước   |
| OD004              | HD002        | Sách    |
| OD005              | HD002        | Bút chì |
