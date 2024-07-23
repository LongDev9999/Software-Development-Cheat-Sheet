# SMOKE TESTING

Smoke Testing là loại kiểm thử để đảm bảo các chức năng chính của ứng dụng là hoạt động tốt. Loại kiểm thử này cũng được biết đến như là "Build Verification Testing". Nó là kiểu kiểm thử không đầy đủ với các trường hợp kiểm tra rất hạn chế nhằm đảm bảo những tính năng quan trọng hoạt động đúng và sẵn sàng để test chi tiết

Smoke Testing được bắt nguồn từ **hardware testing.** Tương tự, khi chúng ta bắt đầu smoke testing của một ứng dụng, điều này nghĩa là chúng ra đang cố gắng để đảm bảo rằng không nên có bất kì lỗi nghiêm trọng nào trước khi đưa đưa ra bản build cho việc kiểm thử đầy đủ

- Mục đích của Smoke Testing là đảm bảo rằng các chức năng quan trọng của ứng dụng là hoạt động tốt
- Đây là kiểm thử không đầy đủ với rất ít số lượng test case
- Nó được biết tới như "Build Verification Testing", nơi mà bản build được xác định bởi việc kiểm tra các tính năng quan trọng của ứng dụng và sau đó được báo cáo rằng nó là tốt để chuyển giao tới kiểm thử chi tiết
- Smoke Testing thường được sử dụng với "positive scenarios" và các dữ liệu hợp lệ
- Nó là một loại của kiểm thử nông và rộng bởi nó được bảo phủ tất cả các trường hợp cơ bản và các chức năng quan trọng của dự án
- Smoke Testing giống như việc kiểm tra sức khoẻ bình thường của một ứng dụng

**Ví dụ**: Giả sử có một ứng dụng Quản lý nhân viên bao gồm 15 modules, trong đó có 4 tính năng chính: Đăng nhập, Thêm mới nhân viên, Sửa thông tin nhân viên, Xoá nhân viên. Smoke Testing chính là chúng ta sẽ kiểm tra đăng nhập với giá trị hợp lệ, sau khi đăng nhập thành công, chúng ta sẽ kiểm tra thêm mới, sửa và xoá thông tin nhân viên. Nếu 4 tính năng quan trọng này hoạt động tốt, thì bản build lúc đó được coi là đủ ổn định để tiến hành kiểm thử chi tiết.

**Khi nào sử dụng Smoke Testing?**

- Nó được hoàn thành bởi developers trước khi đưa bản build cho team QC

![img](https://blog.pirago.vn/content/images/2022/04/image-14.png)

- Nó được hoàn thành bởi Testers trước khi họ kiểm tra kiểm thử chi tiết

![img](https://blog.pirago.vn/content/images/2022/04/image-12.png)

- Smoke Testing được hoàn thành để đảm bảo các chức năng cơ bản của ứng dụng là hoạt động tốt

**Ưu điểm của Smoke Testing**

![img](https://blog.pirago.vn/content/images/2022/04/image-16.png)

- Nó giúp tìm ra bugs trong giai đoạn kiểm thử sớm
- Nó giúp tìm ra các vấn đề được đưa ra bởi tích hợp các thành phần
- Nó giúp xác định các vấn đề được sửa ở bản build trước là không ảnh hưởng tới các chức năng cơ bản của ứng dụng
- Rất hạn chế số lượng test cases được yêu cầu để làm smoke testing
- Smoke Testing có thể được tiến hành trong thời gian rất ít

**Nhược điểm của Smoke Testing**

![img](https://blog.pirago.vn/content/images/2022/04/image-18.png)

- Smoke Testing không bao gồm kiểm thử chi tiết
- Nó là kiểm thử không đầy đủ với số lượng ít test case bởi vậy nên chúng ta không có khả năng để tìm ra các vấn đề quan trọng
- Smoke Testing là **không được thực hiện với "negative scenarios" và các giá trị không hợp lệ**