# Alpha testing & Beta testing

## ***\*Các giai đoạn thử nghiệm\****

Các thử nghiệm Alpha và Beta thường được thực hiện cho phần mềm “off-the-shelf” hoặc các công ty product. Các giai đoạn thử nghiệm cho một công ty product thường thay đổi từ một tổ chức định hướng dịch vụ. Sau đây là các giai đoạn thử nghiệm được áp dụng bởi các công ty product

![Thử nghiệm Alpha Vs Thử nghiệm Beta](https://www.guru99.com/images/TestingPhase.png)

***\*Pre-Alpha\****: Giao diện người dùng đã hoàn tất. **Nhưng không phải tất cả các tính năng đều được hoàn thành. Ở giai đoạn này, phần mềm không được xuất bản.**

***\*Alpha\****: Phần mềm sắp hoàn thành và được kiểm tra nội bộ.

***\*Beta\****: Phần mềm ổn định và được phát hành cho một cơ sở người dùng hạn chế. Mục đích là để có được phản hồi của khách hàng về sản phẩm và thực hiện các thay đổi trong phần mềm cho phù hợp.

***\*Release Candidate (RC):\**** Dựa trên phản hồi của Beta Test, thực hiện kiểm tra và fix bug. Ở giai đoạn này, không thực hiện các thay đổi căn bản về chức năng.

***\*Release:\**** phát hành ứng dụng, phần mềm.

## ***\*Thử nghiệm Alpha là gì?\****

***\*Alpha Testing\**** là một loại kiểm thử chấp nhận; được thực hiện để xác định tất cả các vấn đề và lỗi có thể xảy ra trước khi phát hành sản phẩm cuối cùng cho người dùng cuối. Thử nghiệm alpha được thực hiện bởi những người thử nghiệm là nhân viên nội bộ của tổ chức. Mục tiêu chính là xác định các tác vụ mà người dùng thông thường có thể thực hiện và kiểm tra chúng.

Nói một cách đơn giản nhất có thể, loại thử nghiệm này được gọi là alpha chỉ vì nó được thực hiện sớm, gần cuối quá trình phát triển phần mềm và trước khi thử nghiệm beta. Trọng tâm chính của thử nghiệm alpha là mô phỏng người dùng thực bằng cách sử dụng các kỹ thuật hộp đen và hộp trắng.

![Thử nghiệm Alpha Vs Thử nghiệm Beta](https://www.guru99.com/images/AlphaBetaTestingPhase.png)

## ***\*Thử nghiệm Beta là gì?\****

***\*Beta Testing\**** được thực hiện bởi "người dùng thực" của ứng dụng phần mềm trong "môi trường thực". Đây là thử nghiệm cuối cùng trước khi release cho khách hàng.

Phiên bản beta của phần mềm được phát hành cho một số lượng hạn chế người dùng cuối của sản phẩm để có được phản hồi về chất lượng sản phẩm. Thử nghiệm beta làm giảm rủi ro lỗi sản phẩm và tăng chất lượng sản phẩm thông qua xác nhận của khách hàng.

![img](https://blog.pirago.vn/content/images/2023/06/image-12.png)

## ***\*Tiêu chí đầu vào cho thử nghiệm Alpha:\****

- Tài liệu yêu cầu phần mềm hoặc Đặc tả yêu cầu
- Testcases cho tất cả các yêu cầu
- Test team nắm rõ về ứng dụng phần mềm
- Môi trường test.
- Công cụ quản lý kiểm thử.
- Ma trận truy xuất nguồn gốc để đảm bảo rằng mỗi yêu cầu thiết kế có một testcase tương ứng.

## ***\*Tiêu chí đầu vào để thử nghiệm beta:\****

- Tài liệu về thử nghiệm Alpha
- Phiên bản beta của phần mềm
- Môi trường sẵn sàng phát hành ứng dụng phần mềm cho công chúng
- Công cụ để nắm bắt lỗi thời gian thực

## ***\*Tiêu chí\** chấp nhận \**để thử nghiệm Alpha\****

- Tất cả các trường hợp kiểm thử đã được thực hiện và thông qua.
- Tất cả các vấn đề nghiêm trọng cần phải được khắc phục và close
- Cung cấp báo cáo tóm tắt thử nghiệm
- Đảm bảo rằng không thể bao gồm thêm tính năng bổ sung nào
- Đăng xuất thử nghiệm Alpha

## ***\*Tiêu chí\** chấp nhận \**để thử nghiệm beta:\****

- Tất cả các vấn đề lớn và nhỏ đều được close
- Báo cáo phản hồi từ công chúng
- Cung cấp báo cáo tóm tắt thử nghiệm Beta

## ***\*Ưu điểm của Alpha Testing:\****

- Cung cấp cái nhìn tốt hơn về độ tin cậy của phần mềm ở giai đoạn đầu
- Giúp mô phỏng hành vi và môi trường người dùng theo thời gian thực.
- Phát hiện nhiều showstopper (lỗi làm ngưng hệ thống) hoặc lỗi nghiêm trọng
- Khả năng cung cấp phát hiện sớm các lỗi liên quan đến thiết kế và chức năng

## ***\*Ưu điểm của thử nghiệm Beta\****

- Giảm rủi ro lỗi sản phẩm thông qua xác thực của khách hàng.
- Thử nghiệm beta cho phép một công ty thử nghiệm cơ sở hạ tầng sau khi release.
- Cải thiện chất lượng sản phẩm thông qua phản hồi của khách hàng
- Hiệu quả về chi phí so với các phương pháp thu thập dữ liệu tương tự
- Tạo thiện chí với khách hàng và tăng sự hài lòng của khách hàng

## ***\*Nhược điểm của Alpha Testing:\****

- Về chiều sâu, chức năng không thể được kiểm tra vì phần mềm vẫn đang trong giai đoạn phát triển
- Đôi khi các developer và tester không hài lòng với kết quả của thử nghiệm alpha

## ***\*Nhược điểm của thử nghiệm Beta\****

- Khó khăn trong quản lý kiểm thử.
- Khó khăn trong tìm kiếm đối tượng khách hàng chất lượng duy trì thực hiện Beta testing.

## **Kết luận:**

Trong Kỹ thuật phần mềm, dù thực hiện test rất kĩ càng hay phát hiện được nhiều bug, phần mềm sẽ vô dụng nếu người dùng cuối không hài lòng. Thử nghiệm beta giúp cung cấp phản hồi xác thực về phần mềm từ người dùng thực.

Trong khi đó, thử nghiệm Alpha giúp mô phỏng môi trường người dùng thời gian thực và đảm bảo phần mềm ổn định trước khi phần mềm được gửi đi Thử nghiệm Beta.