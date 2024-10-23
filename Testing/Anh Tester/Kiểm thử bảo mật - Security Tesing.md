## Kiểm thử bảo mật - Security Tesing

Với một trang web có dữ liệu khổng lồ như ngân hàng, bệnh viện... nếu một ngày chúng bị đánh cắp thông tin thì bạn nghĩ hậu quả như thế nào? Thông tin cá nhân cũng như thông tin giao dịch hay thông tin bệnh nhân sẽ bị tiết lộ. Liệu một khi chúng phát tán ra ngoài thì hậu quả như thế nào? Thật đáng lo ngại về nó.

Vậy thì làm sao để tránh các trường hợp lộ, rò rỉ thông tin? Một bước quan trọng khi kiểm thử đó là kiểm thử về Security mà mỗi Tester - Người kiểm thử phần mềm phải biết. Hôm nay chúng ta cùng Anh Tester đi tìm hiểu về các thuật ngữ được sử dụng trong kiểm thử bảo mật trang web và các phương pháp.

## 1. Kiểm thử bảo mật là gì?

**Kiểm thử bảo mật** là kiểm tra xem dữ liệu có giữ bí mật được hay không và trong hệ thống phần mềm thì người dùng sẽ chỉ dùng được các chức năng mà họ được cho phép sử dụng. Ví dụ: Hệ thống quản lý nhân sự thì nhân viên này không thể xem thông tin chi tiết của nhân viên khác, chỉ người nào quản lý mới được xem thông tin. Một số thuật ngữ được sử dụng trong kiểm thử bảo mật

**"Vulnerability" là gì?**

Đây là điểm yếu trong ứng dụng website. Nó là lỗi trong ứng dụng, mã SQL / script hoặc sự hiện diện của virus.

**"URL Manipulation" là gì?**

Như chúng ta đã biết thì một số ứng dụng web giao tiếp thông tin giữa máy khách (trình duyệt) và máy chủ (server) qua URL. Trong trường hợp chúng ta thực hiện thay đổi một số thông tin trong URL thì nó có thể dẫn đến hành vi ngoài ý muốn của máy chủ - Đây được gọi là thao tác URL.

**“SQL injection” là gì?**

Đây là quá trình người dùng cố ý chèn các câu lệnh SQL thông qua giao diện người dùng ứng dụng web vào với một số câu lệnh truy vấn sau đó được máy chủ thực thi.

**“XSS (Cross-Site Scripting)” là gì?**

Khi một người dùng chèn tập lệnh html ở phía máy khách trong giao diện của ứng dụng web, phần chèn này hiển thị cho người dùng khác và nó được gọi là XSS.

**“Spoofing” là gì?**

Đó là việc tạo ra các trang web hoặc email giống như trò lừa bịp được gọi là Spoofing.



Kiểm tra bảo mật của bất kỳ hệ thống nào đều tập trung vào việc tìm ra tất cả các lỗ hổng và điểm yếu trong hệ thống có thể dẫn đến việc mất thông tin hoặc danh tiếng của tổ chức.

### Mục tiêu của kiểm tra bảo mật là:

- Để xác định các mối đe dọa trong hệ thống.
- Để đo lường các lỗ hổng tiềm ẩn của hệ thống.
- Để giúp phát hiện mọi rủi ro bảo mật có thể có trong hệ thống.
- Để giúp các nhà phát triển khắc phục các vấn đề bảo mật thông qua mã hóa.

### Các lĩnh vực trọng tâm chính trong kiểm tra bảo mật:

- An ninh mạng
- Bảo mật phần mềm hệ thống
- Bảo mật ứng dụng phía khách hàng
- Bảo mật ứng dụng phía máy chủ

##  2. Các loại kiểm thử bảo mật

1. Rà soát các lỗ hổng tiềm ẩn: lỗ hổng được thực hiện với sự trợ giúp của phần mềm tự động để quét một hệ thống nhằm phát hiện các mẫu lỗ hổng đã biết.
2. Rà soát các điểm yếu của hệ thống: bao gồm việc xác định các điểm yếu của mạng và hệ thống. Sau đó, nó cung cấp các giải pháp để giảm những khiếm khuyết hoặc rủi ro này. Quét an ninh có thể được thực hiện theo cả cách thủ công và tự động.
3. Đánh giá bảo mật bằng cách tấn công vào hệ thống: là loại kiểm thử mô phỏng cuộc tấn công từ phía một hacker mũ đen. Kiểm thử bao gồm việc phân tích một hệ thống cụ thể, tìm ra các lỗ hổng tiềm ẩn bằng cách tấn công từ bên ngoài.
4. Đánh giá rủi ro: kiểm thử này liên quan đến phân tích các rủi ro bảo mật nhận thấy được. Các rủi ro được phân loại là Low, Medium, High. Loại kiểm thử này đưa ra các khuyến nghị nhằm giảm thiểu các rủi ro.
5. Kiểm tra an ninh nội bộ hệ thống: kiểm tra bảo mật nội bộ ứng dụng và OS. Việc kiểm tra cũng có thể được thực hiện thông qua kiểm tra từng dòng mã.
6. Tấn công vào hệ thống tìm các điểm yếu bảo mật: các hacker mũ trắng thực hiện phương pháp tương tự như những hacker mũ đen, với mục tiêu tìm kiếm các điểm yếu bảo mật và xác định cách thức để thâm nhập vào mục tiêu, nhằm đánh giá mức độ thiệt hại do các lổ hỗng này gây ra, từ đó đưa ra cảnh báo cùng những phương án gia cố, kiện toàn bảo mật thích hợp.
7. Posture assessment: Kết hợp quét bảo mật, hack hệ thống một cách có đạo đức, đánh giá rủ ro và tấn công vào hệ thống tìm các điểm yếu bảo mật để đánh giá bảo mật tổng thể của một tổ chức.

##  3. Một số lưu ý khi kiểm thử bảo mật

Để kiểm thử bão mật cho ứng dụng web thì tester cần có kiến thức tốt về giao thức HTTP. Và cũng cần phải biết trình duyệt và server giao tiếp bằng HTTP. Ngoài ra, tester cũng nên biết những điều cơ bản về SQL và XSS.

##  4. Một số phương pháp để kiểm thử bảo mật

- **Password Cracking - Bẻ khóa mật khẩu**

Chắc chúng ta nghe nhiều về việc bẻ khóa. Vì vậy chúng ta cần phải kiểm tra bảo mật xem web có bị bẻ khóa hay không. Ví dụ khi đăng nhập vào hệ thống, người ta có thể đoán tên người dùng/ mật khẩu hoặc sử dụng công cụ bẻ khóa mật khẩu. Một danh sách các tên người dùng và mật khẩu phổ biến có sẵn cùng với các công cụ bẻ khóa mật khẩu nguồn mở.

Nếu ứng dụng web không thực thi một mật khẩu phức tạp (Ví dụ: với bảng chữ cái, chữ in hoa, in thường, số và ký tự đặc biệt ), có thể không mất nhiều thời gian để bẻ khóa tên người dùng và mật khẩu. Nếu tên người dùng hoặc mật khẩu được lưu trữ trong cookie mà không cần mã hóa, kẻ tấn công (hacker) có thể sử dụng các phương pháp khác nhau để đánh cắp cookie và thông tin được lưu trữ trong cookie như tên người dùng và mật khẩu.

- **Thao tác URL thông qua các phương thức HTTP GET**

Đối với một tester nên kiểm tra xem ứng dụng có truyền thông tin quan trọng trong chuỗi truy vấn hay không. Nó xảy ra khi sử dụng phương thức HTTP GET để truyền thông tin giữa máy khách và máy chủ. Thông tin được truyền qua các tham số trong chuỗi truy vấn. Người kiểm tra có thể sửa đổi một giá trị tham số trong chuỗi truy vấn để kiểm tra xem máy chủ có chấp nhận nó không.

Thông qua HTTP GET yêu cầu thông tin người dùng được chuyển đến máy chủ để xác thực hoặc tìm nạp dữ liệu. Kẻ tấn công có thể thao tác mọi biến đầu vào được truyền từ yêu cầu GET này đến máy chủ để lấy thông tin cần thiết.

- **SQL Injection**

Chúng ta nghe rất nhiều về các cuộc tấn công của hacker từ SQL. Vậy tấn công SQL là gì? Vì sao nó lại ảnh hưởng lớn? Các cuộc tấn công SQL rất quan trọng vì kẻ tấn công có thể lấy thông tin quan trọng từ cơ sở dữ liệu máy chủ. Để kiểm tra các điểm nhập SQL vào ứng dụng web của bạn, hãy tìm hiểu mã từ cơ sở mã của bạn nơi các truy vấn trực tiếp của MySQL được thực thi trên cơ sở dữ liệu bằng cách chấp nhận một số đầu vào của người dùng.

Nếu dữ liệu đầu vào của người dùng được tạo trong các truy vấn SQL để truy vấn cơ sở dữ liệu, kẻ tấn công có thể tiêm các câu lệnh SQL hoặc một phần của các câu lệnh SQL làm đầu vào của người dùng để trích xuất thông tin quan trọng từ cơ sở dữ liệu. Ngay cả khi kẻ tấn công thành công để đánh sập ứng dụng, từ lỗi truy vấn SQL hiển thị trên trình duyệt, kẻ tấn công có thể lấy thông tin mà chúng đang tìm kiếm.

- **Cross-Site Scripting (XSS)**

Với một tester thì cũng phải kiểm thử về XSS của trang web. Kẻ tấn công có thể sử dụng phương pháp này để thực thi tập lệnh hoặc URL độc hại trên trình duyệt bị tấn công. Với XSS, kẻ tấn công có thể sử dụng các tập lệnh như JavaScript để đánh cắp cookie của người dùng và thông tin được lưu trữ trong cookie. Kẻ tấn công có thể dễ dàng vượt qua một số đầu vào độc hại hoặc <script> dưới dạng tham số và truy vấn có thể khám phá dữ liệu người dùng / máy chủ quan trọng trên trình duyệt.



## 5. Một số công cụ hỗ trợ kiểm thử bảo mật

- **Acunetix**

Bạn có thể tìm hiểu thêm thông tin ở đây: https://www.acunetix.com/web-vulnerability-scanner/

- **Kiuwan**

Kiuwan tuân thủ các tiêu chuẩn bảo mật nghiêm ngặt nhất bao gồm OWASP, CWE, Sans 25, HIPPA, v.v. Kiuwan là công cụ hỗ trợ tất cả các ngôn ngữ lập trình và tích hợp với các công cụ DevOps hàng đầu.

- **WireShark**

WireShark là một công cụ phân tích mạng trước đây được gọi là Ethereal. Nó chụp gói tin trong thời gian thực và hiển thị chúng ở định dạng có thể đọc được. Về cơ bản, nó là một bộ phân tích gói mạng - cung cấp các chi tiết nhỏ nhất về các giao thức mạng, giải mã, thông tin gói, v.v ... Nó là một mã nguồn mở và có thể được sử dụng trên Linux, Windows, OS X, Solaris, NetBSD, FreeBSD và nhiều các hệ thống khác.

- **Owasp**

OWASP là một tiêu chuẩn để phục vụ việc kiểm thử của Penetration Testing (Pentest) do tổ chức Open Web Application Security Project(OWASP) đề xuất. OWASP là tổ chức phi lợi nhuận và đưa ra chuẩn OWASP phục vụ cho công việc pentest hiệu quả và chi tiết. Tuy nhiên, để rõ hơn, mình xin giới thiệu sơ qua Pentest là gì.

OWASP là một tổ chức phi lợi nhuận trên toàn thế giới tập trung vào việc cải thiện tính bảo mật của phần mềm. Dự án có nhiều công cụ để kiểm tra các môi trường và giao thức phần mềm khác nhau. Các công cụ hàng đầu của dự án bao gồm:

- Zed Attack Proxy (ZAP - một công cụ tự động tìm các lỗi bảo mật trong khi bạn đang phát triển và thử nghiệm ứng dụng)

- Kiểm tra phụ thuộc OWASP (quét các phụ thuộc của dự án và kiểm tra các lỗ hổng đã biết)

- Dự án môi trường thử nghiệm web OWASP (bộ sưu tập các công cụ và tài liệu bảo mật)

  

- **W3af**

W3af là một framework giúp kiểm tra và xác định các lỗ hổng trong các ứng dụng web. Công cụ này đi kèm với một số plugin hữu ích để quét một trang web với hơn 200 lỗ hổng công khai. Các plugin hiện có sẵn bao gồm kiểm tra, xác thực, bruteforce, thu thập thông tin, trốn, grep và cơ sở hạ tầng. Mỗi plugin có một bộ mục tiêu quét khác nhau.

*
Trên đây là một số cách kiểm thử bảo mật mà mỗi tester nên biết. Cám ơn các bạn đã đọc bài viết, mong nó sẽ có ích đối với bạn.*