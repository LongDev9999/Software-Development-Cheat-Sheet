## MỘT SỐ BUG THƯỜNG GẶP TRONG QUÁ TRÌNH TEST WEB APPLICATION

Các bạn có thể tham khảo và bổ sung cho mình một Checklist để testing riêng nhé !!!



## I. MỘT SỐ LƯU Ý VỀ BUG

***Khi log Bug, bước xác định rất quan trọng:***

- **What** - Bug này là bug gì, độ nghiêm trọng của nó như thế nào?
- **Where** - Xác định lỗi ở đâu, trên môi trường nào (web thì browser nào, app thì trên hệ điều hành nào)
- **When** - Bug xảy ra khi nào (nghĩa là thực hiện những bước nào thì xảy ra Bug)
- **How** - Nó sẽ như thế nào thì mới Đúng (expected result)
- **Who** – Bug do code của ai gây ra?


Tìm ra Bug của phần mềm là chưa đủ, cần phải xem Bug đó đã được fix hay chưa, các bước tái hiện lại bug đó và đặc biệt: việc fix Bug đó không gây ra Bug mới.

Không phải tất cả các Bug tìm ra đều được fix: Cần phải đánh giá độ quan trọng của Bug xem Bug nào cần phải fix, nên fix và bug nào không cần fix.

 

## II. CÁC LỖI THƯỜNG GẶP TRONG QUÁ TRÌNH TEST WEB

### 1. Lỗi về chức năng (Function Bug)

***(Tương ứng là loại Bug - Độ ưu tiên)\***

- Link từ trang này đến trang khác không hoạt động - **High**
- Link từ trang này đến trang khác bị sai - **High**
- Lỗi khi nhập các thẻ HTML, kí tự đặc biệt, kí tự mở rộng…vào các ô Textbox - Medium
- Không check các trường nhập liệu liên quan quan đến ngày tháng - Medium
- Không hiển thị hoặc hiển thị sai các thông báo lỗi khi xảy ra lỗi nhập liệu trên màn hình - Medium
- Dữ liệu cũ được thực hiện nhiều lần: browser back, F5... - Medium
- Có thông báo thực hiện xong chức năng nhưng dữ liệu không được ghi vào DB - **High
  **
- Đưa vào một lượng lớn dữ liệu làm chương trình không chạy được - **High
  **
- Nhập sai kiểu dữ liệu làm hệ thống xảy ra lỗi không lưu vào database được - **High**
- Lỗi chưa verify Button đã được hiển thị khi chưa nhập đủ các trường bắt buộc - Medium
- Lỗi Notify thông báo chưa sắp xếp theo thứ tự mới nhất - Medium

### ** **2. Lỗi về bảo mật (Security Bug)

- Từ một trang hiện tại, thay đổi một số thuộc tính trên link thì có thể đến một trang khác mà người dùng không có quyền truy cập - **High**
- User đã out khỏi hệ thống, browser back nhưng vẫn có thể thực hiện các chức năng - **High
  **
- Hệ thống share link cho người dùng hiển thị sai chức năng so với permision được cấp - **High**

### ** **3. Lỗi giao diện (Interface Bug)

- Cách trình bày website không đồng nhất: font chữ, màu sắc,.. - Medium
- Kích thước các ô textbox bị hạn chế (fix cứng) các giá trị trong các ô đó không được hiển thị đầy đủ - Medium
- Layout bị hỏng khi mở lên các môi trường (browser) khác nhau - **High**
- Các câu thông báo sai chính tả - Medium
- Button không chuyển sang màu xám khi bị disable - Medium
- Tên các button, link….mang tính kĩ thuật, không dễ hiểu với người dùng - Medium
- Popup nhiều lớp, khi chưa đóng cái sau cùng mà vẫn click hoặc đóng được lớp trước nó - Low
- Các button hoặc label khác loại mà giống nhau tất cả về màu sắc - Low
- Lỗi Notify thông báo, khi click xem rồi chưa chuyển màu (từ đậm sang bình thường) - Low

### ** **4. Lỗi khác (Others Bug)

- Khi có nhiều user cùng truy cập thì hệ thống không đáp ứng được yêu cầu (**performance**).
- Thiếu kí tự (*) bên cạnh các trường bắt buộc.
- Lỗi nhấn Login 2 lần mới vào được hệ thống.


*Trên đây là một số Bug trên Website mà Anh Tester tổng hợp với kinh nghiệm cũng như tham khảo được thêm. Sẽ được update tiếp trong thời gian tới với kinh nghiệm dày hơn nhé !!!*