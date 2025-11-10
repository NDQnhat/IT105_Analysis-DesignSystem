# Hệ thống Quản lý Thư viện - Danh sách lớp

## 1. Class: Book (Sách)
**Vai trò:** Đại diện cho thông tin của mỗi cuốn sách trong thư viện.  

**Thuộc tính (Attributes):**
- `bookID` : Mã sách
- `title` : Tên sách
- `author` : Tác giả
- `publicationYear` : Năm xuất bản
- `isAvailable` : Tình trạng sách (có sẵn / đã cho mượn)

**Phương thức (Methods):**
- `borrow()` : Đánh dấu sách là đã cho mượn
- `returnBook()` : Đánh dấu sách là đã trả

---

## 2. Class: Reader (Độc giả)
**Vai trò:** Đại diện cho người mượn sách từ thư viện.  

**Thuộc tính:**
- `readerID` : Mã độc giả
- `name` : Tên độc giả
- `borrowedBooks` : Danh sách sách đang mượn

**Phương thức:**
- `borrowBook(book: Book)` : Mượn sách
- `returnBook(book: Book)` : Trả sách

---

## 3. Class: LibraryStaff (Nhân viên thư viện)
**Vai trò:** Đại diện cho nhân viên quản lý các hoạt động của thư viện.  

**Thuộc tính:**
- `staffID` : Mã nhân viên
- `name` : Tên nhân viên
- `position` : Chức vụ

**Phương thức:**
- `addBook(book: Book)` : Thêm sách mới vào thư viện
- `removeBook(book: Book)` : Xóa sách khỏi thư viện
- `manageReader(reader: Reader)` : Quản lý thông tin độc giả

---

## 4. Class: Library (Thư viện)
**Vai trò:** Quản lý toàn bộ hoạt động của thư viện, bao gồm sách, độc giả, và nhân viên.  

**Thuộc tính:**
- `books` : Danh sách tất cả sách
- `readers` : Danh sách độc giả
- `staffs` : Danh sách nhân viên

**Phương thức:**
- `lendBook(book: Book, reader: Reader)` : Thực hiện mượn sách
- `receiveBook(book: Book, reader: Reader)` : Thực hiện trả sách
- `addReader(reader: Reader)` : Thêm độc giả mới
- `removeReader(reader: Reader)` : Xóa độc giả
