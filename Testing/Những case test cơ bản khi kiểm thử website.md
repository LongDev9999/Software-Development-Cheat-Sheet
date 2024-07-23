# Những case test cơ bản khi kiểm thử website

1. ***Kiểm thử webiste là gì?***

***\*Kiểm thử website\**** là tên gọi được đặt cho một quá trình kiểm thử phần mềm tập trung vào việc kiểm tra các ứng dụng web.Hay được hiểu đơn giản hơn là kiểm tra ứng dụng web của bạn để tìm lỗi tiềm ẩn trước khi deloy lên môi trường production

### 2. *Những case test cơ bản*

#### **2.1 Check layout tổng quan**

1. Kiểm tra kích thước, màu sắc, hình ảnh, icon…
2. Kiểm tra màu chữ, font chữ của link khi mouse hover, click..
3. Kiểm tra việc phân chia các phần: header, footer, body
4. Trường hợp có ảnh hiển thị trên size thì ảnh phải được resize theo cả 2 chiều
5. Kiểm tra font chữ mặc định của hệ thống

#### **2.2 Check các giá trị default**

1. Kiểm tra sự hiển thị của textbox, textarea… có dòng chữ mờ ở bên trong không. Khi user click vào hoặc nhập text thì dòng chữ mờ có mất đi không. Text được nhập vào màu chữ phải rõ chứ không mờ như chữ default.
2. Kiểm tra việc hiển thị mặc định của các trường combobox, listbox (Thường hiển thị giá trị có sẵn trong combobox).
3. Kiểm tra các giá trị checked default checkbox, radio button.
4. Kiểm tra sự hiển thị mặc định của table khi không có bản ghi nào.
5. Phải có kí tự * ở các trường bắt buộc. Khi thông báo lỗi ở trường nào thì phải focus ở trường đấy.
6. Khi chuyển tab, các trường bị disable thì không được focus vào.
7. Kiểm tra mặc định của các button khi được disable phải để ở dạng xám mờ, khi mouse hover thì không có dấu hiệu chứa thẻ.

#### 2.3 Kiểm tra function

***Textbox\***

1. Kiểm tra các giá trị biên của textbox
2. Kiểm tra các giá trị hợp lệ
3. Kiểm tra khi nhập các kí tự HTML, Javasript (vd: <html>abc</html> hoặc <script> alert ('Hello') </script>).
4. Kiểm tra khi nhập các kí tự đặc biệt (kí tự @, ~,!,...)
5. Kiểm tra khi nhập giá trị SPACE đầu, cuối/ hoặc để trống
6. Kiểm tra khi thực hiện CTRL+V; CTRL+C; CTRL+X
7. Kiểm tra khi ấn nút TAB thì con trỏ có di chuyển giữa các textbox theo thứ tự từ trái sang phải, từ trên xuống dưới (đối với nhiều textbox)
8. Kiểm tra khi ấn SHIFT+TAB thì con trỏ có di chuyển giữa các textbox theo thứ tự ngược lại, từ phải sang trái, từ dưới lên trên(đối với nhiều textbox) 9.Các textbox Readonly: Tất cả các trường và điều khiển đều không có hiệu lực trong chế độ Read_only không?
9. Text area: Kiểm tra các giá trị biên của field

***Selection box\***

1. Kiểm tra chức năng Sort của các cột trong phần danh sách
2. Kiểm tra các nội dung trong selection box đúng và đủ

***Combobox\***

1. Các đối tượng trong combobox được sắp xếp theo thứ tự alphabet.
2. Cho phép sử dụng phím lên, xuống và phím enter để lựa chọn các đối tượng.
3. Cho phép nhập tìm kiếm theo chữ cái đầu tiền của danh sách các đối tượng
4. Khi nội dung trong nó dài => thêm scroll

***List box\***

1. Dùng chuột để chọn 1 đối tượng trong danh sách
2. Cho phép nhập tìm kiếm theo chữ cái đầu tiền của danh sách các đối tượng
3. Danh sách các đối tượng được sắp xếp theo bảng chữ cái
4. Hiển thị scroll bar ngang và dọc để có thể xem hết được nội dung

***Checkbox\***

1. Kiểm tra nếu Click 1 lần và 2 lần hộp checkbox
2. Kiểm tra có thể không chọn checkbox hoặc chọn một giá trị
3. Kiểm tra chọn nhiều hộp checkbox

***Button\***

Kiểm tra xử lý khi click vào button này (vd: chuyển đến trang khác, thêm, cập nhật, xoá...)

***Table\***

1. Kiểm tra hiển thị table khi không có bản ghi hoặc khi đã có bản ghi rồi
2. Kiểm tra chức năng sort của table

***Scroll bar\***

Kiểm tra hướng của scroll bar (ngang, dọc)

***Pop-up message, dialog, alert\***

1. Kiểm tra pop-up msg được hiển thị ở phía client hay server.
2. Kiểm tra thứ tự thông báo lỗi của các hộp thoại trên trang khi không kết nối được tới DB phải có thông báo cụ thể chứ không được hiển thị ra trang lỗi của trình duyệt. Phải có thông báo lỗi khi xảy ra lỗi nhập liệu trên màn hình.

***Brower- version***

Ví dụ như IE, Firefox, Chrome, Opera mini .. Và các vesion tương ứng của chúng.

***Session\***Kiểm tra session: Sau khi thực hiện xong 1 action phải xóa session nếu không sẽ dẫn tới dữ liệu cũ vẫn được thực hiện nhiều lần khi ấn F5 trên trình duyệt.

***Cookie\***Kiểm tra việc xử lý của cookie

***Check mạng\***Hiển thị thông báo đến user khi mất mạng (dưới dạng alert, dialog,..)

***Phân trang\***

1. **Kiểm tra khi đang ở trang cuối cùng thì link chuyển đến last page bị disable**
2. **Kiểm tra khi đang ở trang đầu tiên thì link chuyển đến first page bị disable**
3. Kiểm tra sự kiện next , previous trang khi có nhiều trang. Di chuyển đến trang tiếp theo trang trước trang đó
4. Kiểm tra khi nhấn vào một trang bất kì. Di chuyển đến trang tương ứng

***
**Search**

1. Search theo toán tử or hoặc not (search thông tin với riêng từng giá trị hoặc phủ định của giá trị trong đó)
2. Search theo toán tử and (tạo ra các bộ tương ứng để thực hiện search)
3. Phân biệt chữ hoa chữ thường, tiếng việt, tiếng anh, .. Khi thực hiện test
4. Khả năng lưu giữ điều kiện tìm kiếm khi thực hiện phân trang