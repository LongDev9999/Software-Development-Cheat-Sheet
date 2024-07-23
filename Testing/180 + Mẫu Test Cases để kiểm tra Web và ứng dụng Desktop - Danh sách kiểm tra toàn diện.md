# 180 + Mẫu Test Cases để kiểm tra Web và ứng dụng Desktop - Danh sách kiểm tra toàn diện

Đây là một danh sách kiểm tra thử nghiệm cho các ứng dụng web và máy tính để bàn.

Mục tiêu của bài viết là để chia sẻ một trong những danh sách kiểm tra thử nghiệm toàn diện nhất.

Danh sách kiểm tra như một phần không thể thiếu trong các trường hợp kiểm tra quá trình viết. Sử dụng danh sách kiểm tra này, bạn có thể dễ dàng tạo ra hàng trăm trường hợp thử nghiệm để thử nghiệm web hoặc ứng dụng desktop. Đây là tất cả các trường hợp kiểm tra chung và nên được áp dụng cho hầu như tất cả các loại ứng dụng. Tham khảo các thử nghiệm trong khi viết các trường hợp thử nghiệm cho dự án của bạn và chắc chắn sẽ bao gồm hầu hết các loại thử nghiệm, ngoại trừ các quy tắc kinh doanh ứng dụng cụ thể được cung cấp trong tài liệu SRS.

![img](https://images.viblo.asia/d9cd15a8-8003-407a-ac98-0345d60d08cb.gif)

Đây là một danh sách kiểm tra thông thường, bạn nên chuẩn bị một danh sách kiểm tra thử nghiệm tiêu chuẩn phù hợp với nhu cầu cụ thể của bạn sử dụng trường hợp thử nghiệm dưới đây ngoài với các thử nghiệm ứng dụng cụ thể.

## Tầm quan trọng của việc sử dụng checklist cho việc kiểm thử

- Duy trì một kho lưu trữ tiêu chuẩn của các trường hợp thử nghiệm tái sử dụng cho các ứng dụng của bạn sẽ đảm bảo các lỗi phổ biến nhất sẽ bị bắt một cách nhanh chóng hơn.
- Checklist giúp nhanh chóng hoàn tất viết test case các phiên bản mới của ứng dụng.
- Sử dụng lại test case giúp tiết kiệm tiền về nguồn lực để viết kiểm tra lặp đi lặp lại.
- Các trường hợp kiểm tra quan trọng sẽ được đảm bảo luôn luôn làm cho nó gần như không thể quên.
- Kiểm tra checklist có thể bởi dev để đảm bảo các vấn đề phổ biến nhất được cố định trong giai đoạn phát triển bản thân.

**Vài lưu ý cần nhớ:**

1. Thực thi các kịch bản với vai trò người dùng khác nhau ví dụ như người dùng admin, người dùng khách, ...
2. Đối với các ứng dụng web những tình huống này có thể được thử nghiệm trên nhiều trình duyệt như IE, FF, Chrome, và Safari với các phiên bản của khách hàng đã được phê duyệt.
3. Thử nghiệm với độ phân giải màn hình khác nhau như 1024 x 768, 1280 x 1024, ...
4. Ứng dụng nên được thử nghiệm trên nhiều màn hình như màn hình LCD, CRT, điện thoại xách tay, máy tính bảng, và di động.
5. Ứng dụng thử nghiệm trên các nền tảng khác nhau như các hệ điều hành Windows, Mac, Linux.

## Kiểm tra Checklist toàn diện để kiểm tra ứng dụng Web và Desktop

**Giả định** : Giả sử rằng ứng dụng của bạn hỗ trợ chức năng sau:

- Các forms với các trường khác nhau.
- Cửa sổ con.
- Ứng dụng tương tác với cơ sở dữ liệu.
- Tiêu chí tìm kiếm bộ lọc khác nhau và hiển thị kết quả.
- Upload hình ảnh.
- Chức năng gửi email.
- Chức năng xuất dữ liệu.

## Kịch bản thử nghiệm chung

1. Tất cả trường bắt buộc phải được đánh giá và chỉ định bởi biểu tượng dấu hoa thị (*) .
2. Thông báo lỗi validate nên được hiển thị chính xác ở đúng vị trí .
3. Tất cả các thông báo lỗi sẽ được hiển thị trong cùng một phong cách CSS (ví dụ như sử dụng màu đỏ) .
4. Xác nhận chung thông điệp sẽ được hiển thị sử dụng phong cách CSS khác hơn so với thông báo kiểu lỗi (ví dụ như sử dụng màu xanh lá cây) .
5. Công cụ lời khuyên văn bản phải có ý nghĩa .
6. Trường Dropdown nên nhập đầu tiên là trống hoặc văn bản như 'Select' .
7. Xóa chức năng cho bất cứ hồ sơ trên trang nên yêu cầu xác nhận .
8. Chọn/ bỏ chọn tất cả các hồ sơ tùy chọn cần được cung cấp nếu trang hỗ trợ ghi thêm/ xóa/ cập nhật chức năng .
9. Giá trị tối đa sẽ được hiển thị với các biểu tượng chính xác .
10. Mặc định trang phân loại cần được cung cấp .
11. Cài đặt lại nút chức năng nên thiết lập các giá trị mặc định cho tất cả các trường.
12. Tất cả các giá trị bằng số phải được định dạng đúng .
13. Nhập các trường cần được kiểm tra giá trị trường tối đa. Đầu vào giá trị lớn hơn giới hạn tối đa quy định --> không được chấp nhận hoặc được lưu trữ trong cơ sở dữ liệu .
14. Kiểm tra tất cả các trường đầu vào cho các ký tự đặc biệt .
15. Trường label nên được tiêu chuẩn, ví dụ như trường chấp nhận tên đầu tiên của người dùng phải được dán nhãn đúng là 'First Name'.
16. Kiểm tra phân loại chức năng sau khi thêm / sửa / xóa các hoạt động trên bất kỳ bản ghi.
17. Kiểm tra các chức năng thời gian chờ. Các giá trị thời gian chờ nên được cấu hình. Kiểm tra hành vi ứng dụng sau khi hoạt động thời gian chờ .
18. Kiểm tra các tập tin cookie được sử dụng trong một ứng dụng .
19. Kiểm tra nếu tập tin tải về được trỏ đến sửa đường dẫn tập tin .
20. Tất cả các phím nguồn lực phải được cấu hình trong tập tin cấu hình cơ sở dữ liệu hoặc thay vì mã hóa cứng.
21. Tiêu chuẩn phải được theo sau suốt để đặt tên cho phím nguồn .
22. Xác nhận đánh dấu cho tất cả các trang web (xác nhận HTML và CSS cho các lỗi cú pháp) để chắc chắn rằng nó phù hợp với các tiêu chuẩn .
23. Crash ứng dụng hoặc các trang không có sẵn nên được chuyển đến lỗi trang .
24. Kiểm tra văn bản trên tất cả trang chính tả và lỗi ngữ pháp
25. Kiểm tra các trường đầu vào dạng số với giá trị ký tự đầu vào. Tin nhắn xác nhận thích hợp sẽ xuất hiện .
26. Kiểm tra cho số âm nếu được phép cho trường số .
27. Kiểm tra các trường nhập số với giá trị số thập phân .
28. Kiểm tra chức năng của nút có sẵn trên tất cả các trang .
29. Người dùng không thể submit trang hai lần bằng cách nhấn nút submit liên tiếp nhanh chóng.
30. Chia cho 0 có lỗi nên được xử lý cho bất kỳ tính toán .
31. Dữ liệu đầu vào trống với vị trí đầu tiên và cuối cùng phải được xử lý một cách chính xác.

## GUI và khả năng sử dụng các kịch bản thử nghiệm

1. Tất cả các mục trên trang (ví dụ như hộp văn bản, tùy chọn radio, danh sách thả xuống) nên được sắp xếp đúng.
2. Các giá trị số nên được quyền biện minh trừ khi có quy định khác.
3. Đủ không gian cần được cung cấp giữa các trường nhãn, cột, dòng, thông báo lỗi, ...
4. Thanh Scroll nên được kích hoạt khi cần thiết .
5. Kích thước font chữ, phong cách và màu sắc cho dòng tiêu đề, mô tả văn bản, nhãn, dữ liệu infiled, và thông tin điện lưới nên được tiêu chuẩn theo quy định tại SRS.
6. Mô tả hộp văn bản nên đa đường.
7. Trường Disabled nên được chuyển sang màu xám và người sử dụng không nên thiết lập tập trung vào các trường này.
8. Sau khi bấm vào bất kỳ trường văn bản đầu vào, con chuột mũi tên con trỏ nên được thay đổi để trỏ.
9. Người dùng không nên gõ vào thả xuống chọn danh sách. 10 Thông tin lấp đầy bởi người sử dụng sẽ được giữ nguyên khi có thông báo lỗi trên trang submit. Người sử dụng sẽ nộp submit lại bằng cách sửa chữa các lỗi.
10. Kiểm tra nếu trường nhãn thích hợp được sử dụng trong các thông báo lỗi.
11. Giá trị trường Dropdown sẽ được hiển thị trong định nghĩa thứ tự sắp xếp.
12. Tab và Shift + Tab nên hoạt động đúng.
13. Tùy chọn mặc định radio nên được lựa chọn trước khi load trang.
14. Dòng mức cụ thể và trang trợ giúp thông điệp nên có sẵn.
15. Kiểm tra nếu các trường chính xác đã được nhấn mạnh trong trường hợp lỗi.
16. Kiểm tra xem tùy chọn danh sách thả xuống là có thể đọc được và không phải cắt ngắn nhờ vào trường kích thước giới hạn.
17. Tất cả các nút trên trang nên có thể truy cập bằng phím tắt và người dùng sẽ có thể thực hiện tất cả các hoạt động sử dụng bàn phím.
18. Kiểm tra tất cả các hình ảnh bị broken.
19. Kiểm tra tất cả các trang liên kết hỏng.
20. Tất cả các trang nên có tiêu đề.
21. Thông báo xác nhận sẽ được hiển thị trước khi thực hiện bất kỳ bản cập nhật hoặc xóa các hoạt động.
22. Giờ glass sẽ được hiển thị khi ứng dụng đang bận.
23. Trang văn bản nên để biện minh.
24. Người sử dụng nên có thể chỉ chọn một tùy chọn radio và bất kỳ sự kết hợp với hộp kiểm tra.

## Kịch bản thử nghiệm cho bộ lọc tiêu chuẩn

1. Người sử dụng sẽ có thể lọc kết quả sử dụng tất cả các thông số trên trang chức năng tìm kiếm.
2. Tinh chỉnh nên tải trang tìm kiếm với tất cả người sử dụng lựa chọn các thông số tìm kiếm.
3. Khi có ít nhất một trong các tiêu chí lọc là cần thiết để thực hiện các hoạt động tìm kiếm, đảm bảo đúng thông báo lỗi được hiển thị khi người dùng gửi trang mà không chọn bất kỳ tiêu chí lọc.
4. Khi có ít nhất một trong các tiêu chí lọc lựa chọn không phải là người sử dụng bắt buộc sẽ có thể gửi trang và mặc định tiêu chí tìm kiếm nên được sử dụng để truy vấn kết quả.
5. Tin nhắn xác nhận đúng sẽ được hiển thị cho các giá trị hợp lệ cho tiêu chí lọc.

## Kịch bản thử nghiệm cho lưới kết quả

1. Biểu tượng tải trang sẽ được hiển thị khi nó lấy nhiều hơn thời gian mặc định để tải các trang kết quả.
2. Kiểm tra tất cả các thông số tìm kiếm được sử dụng để lấy dữ liệu hiển thị trên lưới kết quả.
3. Tổng số kết quả sẽ được hiển thị trên lưới kết quả.
4. Tiêu chí tìm kiếm sử dụng để tìm kiếm sẽ được hiển thị trên lưới kết quả.
5. Giá trị lưới kết quả nên được sắp xếp theo cột mặc định.
6. Sắp xếp các cột sẽ được hiển thị với biểu tượng phân loại.
7. Lưới kết quả nên bao gồm tất cả các cột chỉ định với giá trị đúng.
8. Tăng dần và giảm dần phân loại chức năng nên làm việc cho cột được hỗ trợ với các dữ liệu phân loại.
9. Lưới kết quả sẽ được hiển thị với cột thích hợp và khoảng cách giữa các hàng.
10. Phân trang nên được kích hoạt khi có nhiều kết quả hơn so với kết quả mặc định đếm mỗi trang.
11. Kiểm tra trang kế tiếp, trước, đầu tiên và trang cuối chức năng phân trang.
12. Bản ghi trùng lặp không được hiển thị trong kết quả lưới.
13. Kiểm tra tất cả các cột là nhìn thấy và ngang thanh cuộn được kích hoạt nếu cần thiết.
14. Kiểm tra dữ liệu cho cột động (cột có giá trị được tính toán tự động dựa trên các giá trị cột khác).
15. Đối với lưới kết quả cho thấy các báo cáo kiểm tra hàng 'Totals' và xác minh tổng thể cho mỗi cột.
16. Đối với lưới kết quả cho thấy các báo cáo kiểm tra dữ liệu hàng 'Totals' khi pagination được kích hoạt và dùng điều hướng đến trang tiếp theo.
17. Kiểm tra xem các ký hiệu thích hợp được sử dụng để hiển thị các giá trị cột ví dụ như biểu tượng % sẽ được hiển thị để tính tỷ lệ phần trăm.
18. Kiểm tra dữ liệu lưới kết quả nếu phạm vi giá trị ngày được kích hoạt.

## Kịch bản thử nghiệm cho một cửa sổ

1. Kiểm tra xem kích thước cửa sổ mặc định là chính xác.
2. Kiểm tra xem kích thước cửa sổ con là đúng.
3. Kiểm tra nếu có bất kỳ trường trên trang tập trung mặc định (trọng tâm cần được thiết lập trên trường input đầu tiên của màn hình).
4. Kiểm tra xem cửa sổ con đang nhận được đóng vào đóng cửa sổ cha / mở window.
5. Nếu cửa sổ con được mở ra, người sử dụng không nên sử dụng hoặc cập nhật bất kỳ trường trên nền hoặc cửa sổ cha.
6. Kiểm tra cửa sổ tối thiểu, tối đa và chức năng đóng cửa sổ.
7. Kiểm tra nếu cửa sổ khá lớn.
8. Kiểm tra chức năng thanh cuộn cho cửa sổ cha và con.
9. Kiểm tra hủy bỏ chức năng của nút cho cửa sổ con.

## Cơ sở dữ liệu kiểm tra kịch bản thử nghiệm

1. Kiểm tra xem dữ liệu chính xác là nhận được lưu trong cơ sở dữ liệu trên trang submit thành công.
2. Kiểm tra các giá trị cho các cột mà không chấp nhận giá trị null.
3. Kiểm tra tính toàn vẹn dữ liệu. Dữ liệu sẽ được lưu trữ trong một hoặc nhiều bảng dựa trên thiết kế.
4. Tên Index nên được đưa ra theo các tiêu chuẩn như IND <tablename> <ColumnName>.
5. Tables nên có cột chính quan trọng.
6. Cột bảng nên có thông tin mô tả có sẵn ( trừ các cột kiểm toán như ngày tạo ra, tạo ra bởi, ...).
7. Đối với mỗi cơ sở dữ liệu thêm/ cập nhật hoạt động đăng nhập nên được bổ sung.
8. Chỉ mục bảng buộc phải được tạo ra.
9. Kiểm tra, nếu dữ liệu được cam kết cơ sở dữ liệu chỉ khi hoạt động được hoàn thành.
10. Dữ liệu nên được cuộn lại trong trường hợp giao dịch thất bại.
11. Tên cơ sở dữ liệu nên được đưa ra theo các loại ứng dụng thử nghiệm: test, UAT, sandbox, live (mặc dù đây không phải là một tiêu chuẩn, nhưng nó là hữu ích để bảo trì cơ sở dữ liệu).
12. Cơ sở dữ liệu logic tên cần được theo tên cơ sở dữ liệu (hữu ích để bảo trì DB).
13. Thủ tục lưu trữ không nên được đặt tên với tiền tố "sp_".
14. Kiểm tra là giá trị cho các cột kiểm toán bảng (như CreatedDate, createdby, UpdateDate, updatedby, isDeleted, deleteddate, deletedby, ...) là thuộc tính đúng.
15. Kiểm tra xem dữ liệu đầu vào không được cắt ngắn trong khi lưu. Độ dài trường cho thấy người sử dụng trên trang và trong lược đồ cơ sở dữ liệu nên như nhau.
16. Kiểm tra số trường với mức tối thiểu, tối đa, và giá trị thực.
17. Kiểm tra số trường có giá trị âm (cho cả chấp nhận và không chấp nhận).
18. Kiểm tra nếu nút radio và các tùy chọn danh sách thả xuống được lưu trong cơ sở dữ liệu một cách chính xác.
19. Kiểm tra nếu các trường cơ sở dữ liệu được thiết kế với kiểu dữ liệu chính xác và độ dài dữ liệu.
20. Kiểm tra tất cả các ràng buộc bảng: Khóa chính, khóa ngoại, ... được thực hiện một cách chính xác.
21. Kiểm tra thủ tục lưu trữ và trigger với dữ liệu đầu vào mẫu.
22. Trường nhập đầu tiên và dấu spaces nên được cắt ngắn trước khi cam kết dữ liệu vào cơ sở dữ liệu.
23. Giá trị rỗng không được phép trong cột khóa chính.

## Kịch bản thử nghiệm cho hình ảnh tính năng tải lên

(Cũng được áp dụng cho các chức năng upload file khác)

1. Kiểm tra đường dẫn hình ảnh tải lên.
2. Kiểm tra tải lên hình ảnh và chức năng thay đổi hình ảnh.
3. Kiểm tra chức năng tải hình ảnh với các tập tin hình ảnh của các phần mở rộng khác nhau (ví dụ như JPEG, PNG, BMP, ...).
4. Kiểm tra chức năng tải lên hình ảnh với những hình ảnh có không gian hoặc bất kỳ ký tự đặc biệt khác trong tên tập tin.
5. Kiểm tra tải lên hình ảnh có tên trùng lặp.
6. Kiểm tra tải lên hình ảnh với kích thước hình ảnh lớn hơn tối đa kích thước cho phép. Thông báo lỗi thích hợp nên được hiển thị.
7. Kiểm tra chức năng tải hình ảnh với các loại file khác với hình ảnh (ví dụ như txt, doc, pdf, exe,...). Thông báo lỗi thích hợp nên được hiển thị .
8. Kiểm tra nếu hình ảnh của chiều cao và chiều rộng (nếu đã xác định) quy định được chấp nhận nếu không từ chối.
9. Tiến trình tải hình ảnh lên sẽ xuất hiện cho hình ảnh kích thước lớn.
10. Kiểm tra nếu hủy chức năng của nút đang làm việc ở giữa quá trình tải lên.
11. Kiểm tra xem hộp thoại chọn tập tin cho thấy chỉ những tập tin được liệt kê hỗ trợ.
12. Kiểm tra chức năng nhiều hình ảnh tải lên.
13. Kiểm tra chất lượng ảnh sau khi upload. Chất lượng hình ảnh không được thay đổi sau khi tải lên.
14. Kiểm tra xem người dùng có thể sử dụng / xem các hình ảnh tải lên.

## Kịch bản thử nghiệm cho việc gửi email

(Không bao gồm trường hợp thử nghiệm để tạo hoặc xác nhận email ). (Hãy chắc chắn để sử dụng địa chỉ email giả trước khi thực hiện các bài kiểm tra email liên quan).

1. Gửi email mẫu nên sử dụng CSS tiêu chuẩn cho tất cả các email .
2. Địa chỉ Email phải được xác nhận trước khi gửi email.
3. Ký tự đặc biệt trong trường email nên được xử lý đúng cách.
4. Ký tự ngôn ngữ cụ thể (ví dụ như ký tự ngôn ngữ Nga, Trung, Đức) phải được xử lý đúng cách trong trường email.
5. Tiêu đề email không nên để trống.
6. Trường placehoder được sử dụng trong mẫu email phải thay thế bằng giá trị thực tế ví dụ như {FirstName} {Lastname} nên được thay thế với các cá thể đầu tiên và cuối cùng tên đúng cho tất cả người nhận.
7. Nếu báo cáo với các giá trị động mới có trong nội dung email, dữ liệu báo cáo phải được tính toán một cách chính xác.
8. Email tên người gửi không nên được trống.
9. Email nên được kiểm tra trong các khách hàng email khác như Outlook, Gmail, Hotmail, Yahoo! Mail, ...
10. Kiểm tra chức năng gửi email sử dụng TO, CC và BCC.
11. Kiểm tra văn bản email thô.
12. Kiểm tra HTML định dạng email. 13 . Kiểm tra tiêu đề email và footer cho logo của công ty, chính sách bảo mật và các liên kết khác.
13. Kiểm tra email với file đính kèm.
14. Kiểm tra chức năng gửi email tới đơn, đa hoặc phân phối người nhận danh sách.
15. Kiểm tra nếu trả lời vào địa chỉ email là chính xác.
16. Kiểm tra gửi khối lượng lớn các email.

## Kịch bản thử nghiệm cho chức năng Excel Export

1. Tập tin nên được xuất trong hợp phần mở rộng tập tin.
2. Tên tập tin cho tập tin Excel được xuất nên được theo các tiêu chuẩn, ví dụ như nếu tên tập tin được sử dụng dấu thời gian, nó nên được thay thế đúng vào thời điểm thực tế tại thời điểm xuất các tập tin
3. Kiểm tra định dạng ngày nếu tập tin Excel xuất chứa các cột ngày.
4. Kiểm tra số định dạng cho giá trị số hoặc tiền tệ. Định dạng nên được giống như hiển thị trên trang.
5. Tệp tin xuất nên có cột với tên cột thích hợp.
6. Mặc định trang phân loại phải được tiến hành trong tập tin xuất như vậy.
7. Dữ liệu tập tin Excel nên được định dạng đúng với tiêu đề và văn bản footer, ngày, số trang, ... giá trị cho tất cả các trang.
8. Kiểm tra xem dữ liệu hiển thị trên trang và tập tin Excel xuất là như nhau.
9. Chức năng xuất khi pagination được kích hoạt.
10. Kiểm tra nếu nút xuất là hiển thị biểu tượng thích hợp theo loại tập tin xuất biểu tượng như file Excel là xls.
11. Kiểm tra chức năng xuất cho các tập tin có kích thước rất lớn.
12. Kiểm tra chức năng xuất cho các trang có chứa ký tự đặc biệt. Kiểm tra xem các ký tự đặc biệt được xuất đúng trong tập tin Excel.

## Hiệu suất kịch bản thử nghiệm

1. Kiểm tra thời gian tải trang nằm trong phạm vi chấp nhận được.
2. Kiểm tra tải trang trên các kết nối chậm.
3. Kiểm tra thời gian phản ứng đối với bất kỳ hành động dưới ánh sáng, bình thường, trung bình và điều kiện tải nặng.
4. Kiểm tra thực hiện các thủ tục cơ sở dữ liệu được lưu trữ và gây nên.
5. Kiểm tra thời gian thực hiện truy vấn cơ sở dữ liệu.
6. Kiểm tra tải trọng của ứng dụng.
7. Kiểm tra thử nghiệm stress của ứng dụng.
8. Kiểm tra CPU và bộ nhớ sử dụng trong điều kiện tải cao điểm.

## An ninh kiểm tra kịch bản thử nghiệm

1. Kiểm tra các cuộc tấn công SQL injection.
2. Trang an toàn nên sử dụng giao thức HTTPS.
3. Page crash không nên tiết lộ ứng dụng hoặc thông tin máy chủ. Trang lỗi sẽ được hiển thị cho điều này.
4. Thoát ký tự đặc biệt trong đầu vào.
5. Thông báo lỗi không nên tiết lộ bất kỳ thông tin nhạy cảm.
6. Tất cả các thông tin cần được chuyển qua một kênh được mã hóa .
7. An ninh kiểm tra mật khẩu và thực thi chính sách mật khẩu.
8. Kiểm tra chức năng đăng xuất ứng dụng.
9. Kiểm tra cho Brute Force Attacks.
10. Thông tin cookie sẽ được lưu trữ trong chỉ định dạng mã hóa.
11. Kiểm tra thời gian phiên cookie và kết thúc phiên sau khi thời gian chờ hoặc logout.
12. Phiên tokens nên được truyền qua kênh bảo đảm.
13. Mật khẩu không nên được lưu trữ trong cookie.
14. Kiểm tra cho Denial of Service attacks.
15. Kiểm tra bộ nhớ rò rỉ.
16. Kiểm tra ứng dụng truy cập trái phép bằng cách thao tác các giá trị biến trong thanh địa chỉ trình duyệt.
17. Kiểm tra phần mở rộng tập tin bàn giao để các file exe không được tải lên và thực hiện trên máy chủ.
18. Các trường nhạy cảm như mật khẩu và thông tin thẻ tín dụng không nên có tự động hoàn toàn kích hoạt.
19. Tập tin chức năng tải lên nên sử dụng hạn chế loại tập tin và cũng chống virus để quét các tập tin được tải lên.
20. Kiểm tra xem danh sách thư mục bị cấm.
21. Mật khẩu và các trường nhạy cảm khác nên được đeo mặt nạ trong khi gõ.
22. Kiểm tra xem chức năng quên mật khẩu được đảm bảo với các tính năng như tạm thời mật khẩu hết hạn sau giờ quy định và câu hỏi bảo mật được yêu cầu trước khi thay đổi hoặc yêu cầu mật khẩu mới.
23. Xác chức năng CAPTCHA.
24. Kiểm tra xem các sự kiện quan trọng được ghi lại trong các file bản ghi.
25. Kiểm tra nếu truy cập đặc quyền được thực hiện một cách chính xác.

Bài viết này cố gắng để đảm bảo tất cả các kịch bản thử nghiệm tiêu chuẩn cho các chức năng ứng dụng web và máy tính để bàn. Nhưng đây không phải là một danh sách kiểm tra đầy đủ. Với các dự án khác nhau có danh sách kiểm tra thử nghiệm của riêng mình dựa trên kinh nghiệm của tester.