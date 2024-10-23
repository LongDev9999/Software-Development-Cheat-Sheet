## Tìm hiểu về quy trình kiểm thử Website

Bất kỳ công việc gì cũng cần có quy trình kiểm thử riêng nhằm đảm bảo chất lượng sau khi hoàn thành, thiết kế website cũng vậy, mỗi một website trước khi được cho chạy thực tế đều phải trải qua một quy trình kiểm thử chi tiết để đảm bảo không có bất kỳ lỗi nào sẽ phát sinh. Cùng Anh Tester tìm hiểu về quy trình kiểm thử Website ngay sau đây.

## Kiểm thử website là gì?

**Kiểm thử website** là tên gọi được đặt cho một quá trình kiểm thử phần mềm tập trung vào việc kiểm tra các ứng dụng web. Ứng dụng web cần được kiểm tra hoàn toàn trước khi đi vào hoạt động, điều này có thể giúp giải quyết các vấn đề trong ứng dụng web trước khi tiếp xúc với người dùng như các vấn đề về chức năng, bảo mật, các vấn đề dịch vụ web, các vấn đề tích hợp và khả năng xử lý lưu lượng truy cập, trong **quá trình kiểm thử website**, cần cố gắng phát hiện ra lỗi có thể xảy ra trong hệ thống nhằm giải quyết kịp thời. 

*[![Tìm hiểu về quy trình kiểm thử Website | Anh Tester](https://anhtester.com/uploads/post/website_testing_sample.jpg)](https://anhtester.com/uploads/post/website_testing_sample.jpg)
Kiểm thử website là gì?

*

Kiểm thử website chính là kiểm tra xem ứng dụng web có chứa những lỗi tiềm tàng nào không, trước khi chính thức đưa website đi vào sử dụng. Đây là một công việc liên quan đến lập trình web app, các khâu cần kiểm thử đó là bảo mật, chức năng, khả năng xử lý lưu lượng, hiệu suất trang web. 

Nhu cầu sử dụng internet của mọi người tăng cao, do đó việc thiết kế website (ứng dụng web) cũng phát triển rất mạnh mẽ. Website ngày càng đóng vai trò quan trọng trong thương mại điện tử, trao đổi thông tin, giải trí, thư giãn, giới thiệu,… Muốn thiết kế website có hiệu suất sử dụng cao, thì khi sau thiết kế xong, cần phải kiểm thử trang web đó thật cẩn thận, chặt chẽ. Hôm nay Anh Tester sẽ gửi đến các bạn các khâu trong quy trình kiểm thử website.

##  Quy trình kiểm thử Website

 

### **Kiểm thử chức năng website (Functional Testing)**

Trong kiểm thử chức năng ([***Functionality Testing***](https://anhtester.com/blog/functional-testing-kiem-thu-chuc-nang-b284.html)) chúng ta cần kiểm tra từng thành phần hoạt động có như mong đợi hay không, vì vậy nó còn được gọi là “kiểm thử các thành phần”. Kiểm thử chức năng giúp kiểm tra các chức năng của thành phần ứng dung, về cơ bản là để kiểm tra các chức năng được đề cập trong tài liệu mô tả chức năng cũng như kiểm tra xem ứng dụng phần mềm có đáp ứng được kỳ vọng của người dùng hay không.

Các hoạt động kiểm thử này bao gồm:

#### **Kiểm thử liên kết**

Kiểm tra tất cả các liên kết hỏng trên website và tất cả các liên kết đang hoạt động chính xác, bạn có thể kiểm tra các ***liên kết*** khác nhau trên website:

- Liên kết nội bộ
- Liên kết ngoài
- Liên kết mail
- Liên kết anchor

#### ** Kiểm thử web form**

Đây là phần thiết yếu của bất kỳ **kiểm thử website** nào, mục đích chính của kiểm thử web form là lấy thông tin từ người sử dụng và lưu trữ vào cơ sở dữ liệu đồng thời tương tác với lượng dữ liệu ấy. Dưới đây là các trường hợp kiểm thử được nhắc tới trong ***kiểm thử web form\***:

- Điều đầu tiên là kiểm tra tính hợp lệ trên mỗi field của form, dưới đây là hai loại Validation cần được xem xét – “Client side” và “Server side” validations.
- Kiểm tra các giá trị mặc định.
- Kiểm tra tất cả các field bắt buộc.
- Kiểm tra nếu người dùng không nhập vào một field bắt buộc cần hiển thị một thông báo.
- Thêm và sửa thông tin bằng cách sử dụng form.
- Thứ tự các tab trên web form.
- Kiểm tra các giá trị mặc định của field.
- Form cần được định dạng tối ưu khả năng đọc.
- Kiểm tra số âm.

#### ** Kiểm thử Cookie**

Cookie là tập tin chứa thông tin hệ thống của người dùng, các tệp này được lưu ở vị trí mong muốn và được sử dụng bởi các trình duyệt. Các session đăng nhập, thông tin được lưu lại trong cookie (như session) và có thể được truy xuất cho các trang web. Người dùng có thể kích hoạt hoặc vô hiệu Cookies trong các tùy chọn trình duyệt, kiểm thử để kiểm tra xem cookie có được lưu trữ trong máy của người dùng ở định dạng mã hóa hay không. 

- Kiểm tra ứng dụng bằng cách vô hiệu cookies .
- Kiểm tra ứng dụng sau khi hỏng các cookies.
- Kiểm tra hành vi của ứng dụng sau khi xóa tất cả cookie trên website.
- Kiểm tra cookie có hoạt động trên nhiều duyệt khác nhau hay không.
- Kiểm tra cookie cho đăng nhập xác thực có hoạt động hay không.
- Kiểm tra hành vi của ứng dụng sau khi xoá cookie (session) bằng cách xoá bộ nhớ cache hoặc sau khi cookie hết hạn.
- Kiểm tra đăng nhập vào ứng dụng sau khi xóa cookie (session).

#### ** Kiểm thử HTML \*và\* CSS**

Kiểm thử này kiểm tra xem các công cụ tìm kiếm có thể thu thập dữ liệu trang web của bạn mà không xảy ra bất kỳ lỗi nào, bạn nên kiểm tra tất cả các lỗi cú pháp, màu sắc và tuân thử theo tiêu chuẩn như ***[W3C](https://www.w3.org/), ISO***, ECMA, IETF, WS-I, OASIS.

Quy trình nghiệp vụ bao gồm:

- Kiểm tra luồng xử lý đảm bảo sự hoàn chỉnh của website.
- Kiểm tra các màn hình theo như tài liệu yêu cầu.

###  Kiểm thử khả năng sử dụng website (Usability Testing)

Đóng một vai trò quan trọng trong bất kỳ ứng dụng web, ***Usability testing*** đảm bảo kiểm tra tất cả các test case xuất phát từ người dùng. Bao gồm:

#### **Kiểm** **tra điều hướng website**

- Tất cả các tùy chọn như ***UI/UX\***, menu, liên kết hoặc các button trên website phải hiển thị và có thể truy cập.
- Điều hướng trang web dễ dàng sử dụng .
- Nội dung hướng dẫn phải rõ ràng và phải đáp ứng được mục đích.
- Tất cả tùy chọn trên header, footer và các điều hướng trái / phải phải nhất quán trên mỗi trang.

*[![Tìm hiểu về quy trình kiểm thử Website | Anh Tester](https://anhtester.com/uploads/post/kiem-thu-kha-nang-su-dung.png)](https://anhtester.com/uploads/post/kiem-thu-kha-nang-su-dung.png)
kiểm thử khả năng sử dụng trên website

*

#### **Kiểm tra nội dung website**

- Không có lỗi chính tả hoặc ngữ pháp lỗi trong nội dung.
- Tích hợp Alt trong hình ảnh .
- Không có ảnh hỏng.
- Xác nhận tính hợp lệ tất cả giao diện người dùng.
- Thực hiện theo một số tiêu chuẩn về xây dựng nội dung trên trang web.
- Tất cả nội dung phải rõ ràng và dễ hiểu.
- Màu tối gây bất bình cho người sử dụng, vì vậy tránh sử dụng theme màu tối.
- Kích thước hình ảnh kích nên phù hợp.
- Anchor text phải hoạt động bình thường.

### ** Kiểm thử sự tương thích**

Đảm bảo làm thế nào ứng dụng làm việc trong các môi trường được hỗ trợ, sử dụng ứng dụng web trên các hệ điều hành khác nhau, khả năng tương thích của trình duyệt, khả năng tính toán của phần cứng, cơ sở dữ liệu và khả năng xử lý băng thông mạng. Kiểm thử tương thích đảm bảo rằng “ứng dụng web có hiển thị đúng trên các thiết bị khác nhau không?”. Điều này sẽ bao gồm:

*[![Tìm hiểu về quy trình kiểm thử Website | Anh Tester](https://anhtester.com/uploads/post/kiem-thu-su-tuong-thich.png)](https://anhtester.com/uploads/post/kiem-thu-su-tuong-thich.png)
Kiểm tra sự tương thích website*

####  Kiểm tra độ tương thích của trình duyệt

Các ứng dụng web được hiển thị khác nhau trên các trình duyệt khác nhau, mục tiêu của kiểm tra khả năng tương thích của trình duyệt là đảm bảo rằng không có lỗi nào xảy ra trên các trình duyệt web khác nhau trong khi hiển thị website. Bạn cần đảm bảo rằng ứng dụng web của bạn đang được hiển thị đúng trên các trình duyệt khác nhau cũng như kiểm tra AJAX, JavaScript và xác thực hoạt động chính xác.

#### Khả năng tương thích hệ điều hành

Công nghệ mới, sử dụng đồ họa mới hơn, các [API](https://anhtester.com/blog/so-luoc-ve-api-testing-b271.html) khác nhau được sử dụng có thể không hoạt động trên nhiều hệ điều hành, bên cạnh đó các text field, button có thể hiển thị khác nhau trên hệ điều hành khác nhau. Vì vậy, **kiểm thử website** cần được thực hiện trên các hệ điều hành khác nhau như Windows, MAC, Solaris, Unix, Linux.

#### Trình duyệt web di động

Bạn cũng nên kiểm tra khả năng tương thích website trên điện thoại di động, đôi khi có thể xảy ra sự cố tương thích trên các trình duyệt điện thoại di động.

### **Kiểm thử cơ sở dữ liệu**

Độ tin cậy của dữ liệu là một phần quan trọng trong việc kiểm thử cơ sở dữ liệu. Vì vậy, đối với các ứng dụng web nên được kiểm tra một cách kỹ lưỡng. Các hoạt động kiểm tra bao gồm:

*[![Tìm hiểu về quy trình kiểm thử Website | Anh Tester](https://anhtester.com/uploads/post/kiem-thu-co-so-du-lieu.png)](https://anhtester.com/uploads/post/kiem-thu-co-so-du-lieu.png)
kiểm thử website cần độ chính xác từ cơ sở dữ liệu

*

-  Kiểm tra nếu các truy vấn được thực hiện mà không xảy ra lỗi.
-  Thêm mới, cập nhật hoặc xoá dữ liệu trong cơ sở dữ liệu nên duy trì tính toàn vẹn của dữ liệu.
-  Truy vấn dữ liệu không nên mất quá nhiều thời gian.
-  Kiểm tra việc load dữ liệu và kết quả nhận được với các câu truy vấn dài.
-  Dữ liệu nhận được trên cơ sở dữ liệu và hiển thị trên website có chính xác hay không.

### ** Kiểm thử giao diện**

Kiểm thử giao diện chủ yếu có ba lĩnh vực cần được kiểm tra: Web Server, Application server và Database server. Đảm bảo rằng tất cả các thông tin liên lạc giữa các server này phải được thực hiện đúng, xác minh kết nối giữa các máy chủ được thiết lập lại hoặc bị mất, kiểm tra xem có bất kỳ xung đột giữa lúc ứng dụng đang hoạt động, trả về bất kỳ lỗi từ web server hoặc database server đến application server sau đó được xử lý và cuối cùng là hiển thị kết quả tới người dùng.

*[![Kiểm thử giao diện](https://anhtester.com/uploads/post/kiem_thu_giao_dien.png)](https://anhtester.com/uploads/post/kiem_thu_giao_dien.png)
Giao diện chiếm vai trò lớn trong kiểm thử website

*

-  Web server: kiểm tra xem tất cả các yêu cầu web có đang được chấp nhận và không yêu cầu nào bị từ chối hoặc bị rò rỉ.
-  Application server: kiểm tra xem yêu cầu có đang gửi đúng đến server, lỗi có được bắt và hiển thị cho người quản trị.
-  Database server: kiểm tra kết quả truy vấn cơ sở dữ liệu.

### ** Kiểm thử hiệu năng website **

*[![Kiểm thử hiệu năng website](https://anhtester.com/uploads/post/kiem-thu-hieu-nang.png)](https://anhtester.com/uploads/post/kiem-thu-hieu-nang.png)
kiểm thử hiệu năng có ảnh hưởng lớn đối với người dùng

*

Kiểm thử website làm việc dưới lượt tải nặng, được phân thành hai phần: kiểm tra tần suất, kiểm tra lượt tải. Bao gồm:

-  Kiểm tra thời gian phản hồi của website với tốc độ kết nối khác nhau.
-  Kiểm tra website có xử lý được nhiều yêu cầu người dùng vào cùng một thời điểm.
-  Kiểm tra website có hoạt động tốt trong thời điểm lượt tải cao.
-  Kiểm tra dữ liệu đầu vào lớn từ người dùng.
-  Kiểm tra hành vi của website khi kết nối với cơ sở dữ liệu.
-  Kiểm tra các phương pháp tối ưu hóa như giảm thời gian tải bằng cách bật bộ nhớ cache trên trình duyệt và phía máy chủ, nén gzip…

### ** Kiểm thử bảo mật website**

*[![Kiểm thử bảo mật website](https://anhtester.com/uploads/post/kiem_thu_bao_mat.png)](https://anhtester.com/uploads/post/kiem_thu_bao_mat.png)
Kiểm thử bảo mật website

*

Được thực hiện để đảm bảo rằng có bất kỳ rò rỉ thông tin nào về mã hoá dữ liệu hay không. Trong website thương mại điện tử, kiểm thử bảo mật đóng một vai trò rất quan trọng, nếu thông tin an toàn thì kiểm tra xem làm thế nào để lưu trữ các thông tin nhạy cảm như thẻ tín dụng, thanh toán hóa đơn…Các hoạt động kiểm tra sẽ bao gồm:

-  Kiểm tra truy cập trái phép vào các trang an toàn, nếu người dùng thay đổi từ “https” sang “http” thì thông báo thích hợp sẽ được hiển thị và ngược lại.
- Kiểm tra việc truy cập các trang internal, nếu đăng nhập được yêu cầu thì người dùng nên được chuyển hướng đến trang đăng nhập hoặc thông báo thích hợp sẽ được hiển thị.
- Các thông tin liên quan đến giao dịch, thông báo lỗi, cố gắng đăng nhập nên được ghi vào file log.
- Kiểm tra các tệp tin có bị hạn chế tải xuống hay không.
- Kiểm tra các thư mục web hoặc tập tin web có thể truy cập được trừ khi không được cấu hình để tải xuống.
- Kiểm tra CAPTCHA đã được thêm vào và hoạt động bình thường cho đăng nhập để tự động ngăn chặn các đăng nhập hay chưa.
- Kiểm tra việc cố truy cập thông tin bằng cách thay đổi tham số trong chuỗi truy vấn. Ví dụ: nếu bạn đang chỉnh sửa thông tin và trên URL bạn thấy UserID = 123, hãy thử thay đổi các giá trị tham số này và kiểm xem ứng dụng có cung cấp thông tin người dùng khác không, nên từ chối hiển thị cho trường hợp này để ngăn chặn việc xem thông tin người dùng khác.
- Kiểm tra session hết hạn sau thời gian được xác định nếu người dùng không thao tác trên website.
- Kiểm tra user/password không hợp lệ.