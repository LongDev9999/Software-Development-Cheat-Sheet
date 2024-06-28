# Fix bug là gì? Kỹ năng và Tip để Fix bug hiệu quả. Quy trình Fix bug chi tiết

Fix bug xuất hiện trong quá trình phát triển phần mềm, để fix bug không chỉ đòi hỏi [kiến thức](https://wiki.matbao.net/kien-thuc/) kỹ thuật sâu rộng mà còn yêu cầu các kỹ năng phân tích và hiểu rõ về phần mềm.

## **I. Tổng quan về Fix Bug**

### **1. Fix Bug là gì?**

Bug là một khái niệm chỉ các lỗi, sai sót hoặc hành vi không mong muốn trong mã nguồn hoặc phần mềm. Đây có thể là kết quả của lỗi logic, vấn đề về cú pháp, hoặc không đáp ứng đúng các yêu cầu, điều kiện của dự án.

![Tìm hiểu về Fix Bug là gì](https://wiki.matbao.net/wp-content/uploads/2024/01/fix-bug-la-gi.png)

***>>>Xem thêm:[Những cách thức bảo mật website mã nguồn mở trên Cloud Linux Hosting](https://wiki.matbao.net/kb/nhung-cach-thuc-bao-mat-website-ma-nguon-mo-tren-hosting-linux/)<<<\***

Fix Bug là quá trình tìm ra và sửa các lỗi hoặc vấn đề trong mã nguồn của phần mềm hay ứng dụng máy tính.

### **2. Tầm quan trọng của Fix Bug**

- ***Đảm bảo chất lượng:\*** Việc fix bug là một phần quan trọng trong quá trình đảm bảo chất lượng của phần mềm. Nó giúp loại bỏ các lỗi tiềm ẩn hoặc vấn đề có thể ảnh hưởng đến trải nghiệm người dùng.
- ***Tính ổn định:\*** Khi loại bỏ các bug, phần mềm trở nên ổn định hơn, giảm thiểu rủi ro về sự cố không mong muốn khi người dùng sử dụng.
- ***Tăng hiệu suất:\*** Fix bug sớm và hiệu quả có thể ngăn chặn việc tích lũy các vấn đề phức tạp, giúp dự án tiến triển một cách trơn tru hơn.
- ***Nâng cao hình ảnh và uy tín:\*** Việc cải thiện và duy trì chất lượng phần mềm qua việc fix bug liên tục cũng đóng vai trò quan trọng trong việc tạo dựng hình ảnh đáng tin cậy với người dùng.
- ***Tiết kiệm thời gian:\*** Fix bug sớm giúp tránh được việc dành quá nhiều thời gian và tài nguyên cho việc điều chỉnh sau này. Điều này có thể tiết kiệm được cả thời gian lẫn nguồn lực của dự án.

## **II. Kỹ năng cần thiết để fix bug tối ưu**

### **1. Kỹ năng Debugging cho Fix Bug**

#### **Hiểu rõ về các công cụ debugging:**

- ***Debugger:\*** Sử dụng debugger để theo dõi và kiểm tra giá trị biến, flow của chương trình.
- ***Logging:\*** Sử dụng các hệ thống logging để ghi lại thông tin quan trọng trong quá trình chạy ứng dụng, giúp theo dõi và phân tích các sự kiện xảy ra.

![Fix Bug có cần thiết phải biết phân tích lập trình](https://wiki.matbao.net/wp-content/uploads/2024/01/dieu-kien-de-fix-bug.png)

***>>>Xem thêm:[MVC, MVP, MVVM là gì? Thông tin cần biết về các mô hình lập trình](https://wiki.matbao.net/mvc-mvp-mvvm-la-gi-thong-tin-can-biet-ve-cac-mo-hinh-lap-trinh/)<<<\***

- ***Khả năng phân tích stack trace và log:\*** để xác định nguyên nhân bug từ đó fix bug hiệu quả
- ***Stack Trace Analysis:\*** Hiểu và phân tích stack trace để xác định đường dẫn thực thi code khi có bug xảy ra.
- ***Log Analysis:\*** Kiểm tra log files để tìm ra thông tin quan trọng như lỗi, cảnh báo, hoặc dấu hiệu của vấn đề.

### **2. Kiến thức kỹ thuật Fix Bug**

#### **Hiểu biết sâu rộng về ngôn ngữ lập trình và framework sử dụng:**

- ***Ngôn ngữ lập trình:\*** Đặc điểm, cú pháp, và các tính năng đặc biệt của ngôn ngữ.
- ***Framework:\*** Hiểu rõ cấu trúc, quy tắc hoạt động của framework để có cái nhìn tổng quan về cách mà ứng dụng được xây dựng.

#### **Nắm vững các nguyên lý cơ bản về lập trình:**

- ***Quy tắc SOLID\*** (Single Responsibility, Open/Closed, Liskov Substitution, Interface Segregation, Dependency Inversion): Áp dụng các nguyên tắc này để code có tính mở rộng, bảo trì và tái sử dụng tốt hơn.
- ***Design Patterns:\*** Hiểu và áp dụng các mẫu thiết kế phổ biến như Singleton, Factory, Observer để giải quyết vấn đề một cách có cấu trúc và linh hoạt.

## **Tip để Fix Bug nhanh chóng**

### **1. Đọc và hiểu rõ bug report**

#### **Phân tích các thông tin cần thiết từ bug report:**

**Bước 1:** Xác định mô tả chi tiết về vấn đề cụ thể.

- ***Mô tả chính xác vấn đề:\*** Kiểm tra xem bug report có mô tả chi tiết về hành vi không mong muốn hay vấn đề cụ thể xảy ra như thế nào không.
- ***Dữ liệu liên quan:\*** Xác định liệu có dữ liệu cụ thể, thông số nào liên quan đến vấn đề hay không. ***Ví dụ:\*** dữ liệu đầu vào, dữ liệu đầu ra không đúng.

![Để Fix Bug nhanh hơn cần biết những tip nào](https://wiki.matbao.net/wp-content/uploads/2024/01/tip-fix-bug-nhanh.png)

***>>>Xem thêm:[Hướng dẫn sửa lỗi website bị cảnh báo chứa phần mềm độc hại](https://wiki.matbao.net/kb/huong-dan-sua-loi-website-bi-canh-bao-chua-phan-mem-doc-hai/)<<<\***

**Bước 2:** Nhận diện bước tái tạo vấn đề để kiểm tra lại.

- ***Quá trình tái tạo:\*** Kiểm tra xem bug report có cung cấp bước đầy đủ để tái tạo vấn đề hay không. Nếu không, cần liên hệ để đảm bảo việc tái tạo vấn đề được thực hiện chính xác.
- ***Thông tin:\*** Đảm bảo bug report cung cấp thông tin về môi trường và điều kiện để tái tạo vấn đề. Ví dụ: trình duyệt, hệ điều hành, phiên bản phần mềm.

**Bước 3:** Lấy thông tin về môi trường, hệ điều hành, và phiên bản phần mềm liên quan.

- ***Môi trường:\*** Xác định thông tin về môi trường mà bug xảy ra (có thể là production, staging, hay local environment).
- ***Hệ điều hành:\*** Ghi nhận loại và phiên bản hệ điều hành đang được sử dụng.
- ***Phiên bản phần mềm:\*** Xác định phiên bản cụ thể của ứng dụng hoặc phần mềm gây ra vấn đề.

#### **Đặt câu hỏi thêm nếu cần cho quá trình Fix Bug:**

1. Liên hệ với người báo cáo bug để hiểu rõ hơn về quá trình gây ra vấn đề.
2. Yêu cầu thông tin bổ sung để có cái nhìn toàn diện hơn về tình huống.

### **2. Tạo bản sao lưu (backup) trước khi fix bug**

#### **Tạo bản backup trước khi bắt đầu fix bug:**

- ***Codebase:\*** Tạo bản sao lưu của mã nguồn hoặc dự án trước khi thực hiện bất kỳ sửa đổi nào. Điều này có thể bao gồm việc tạo một bản sao lưu của toàn bộ thư mục hoặc repository chứa mã nguồn.
- ***Cơ sở dữ liệu:\*** Trước khi thực hiện các thay đổi trong cơ sở dữ liệu, tạo bản backup đầy đủ của cơ sở dữ liệu. Sử dụng các công cụ như mysqldump (đối với MySQL) hoặc công cụ tương tự để tạo bản sao lưu của cơ sở dữ liệu hiện tại.

#### **Sử dụng công cụ quản lý phiên bản:**

- Sử dụng hệ thống quản lý phiên bản như Git để theo dõi các thay đổi trong mã nguồn. Commit các thay đổi và viết message rõ ràng mô tả nội dung của từng commit.
- Khi cần, có thể sử dụng khả năng rollback của hệ thống quản lý phiên bản để trở về trạng thái trước khi thực hiện thay đổi gây ra vấn đề hoặc bug.

### **3. Chia nhỏ vấn đề và kiểm tra từng phần Fix Bug**

#### **Bước 1: Xác định các Module, Class, hoặc Phần Code**

Xác định các phần của hệ thống hoặc codebase mà vấn đề có thể xuất hiện. Các module, class, hoặc phần code liên quan trực tiếp đến bug cần được xác định.

#### **Bước 2: Phân tích và đưa ra nguyên nhân gây Fix Bug**

Tách vấn đề thành các phần nhỏ hơn để nắm bắt nguyên nhân cụ thể của bug.

Kiểm tra từng module, class, hoặc phần code một cách kỹ lưỡng để xác định điểm gây ra vấn đề.

![Chia nhỏ từng phần để Fix Bug](https://wiki.matbao.net/wp-content/uploads/2024/01/chia-nho-tung-phan-fix-bug.png)

Áp dụng các kỹ thuật debugging như sử dụng log, debugger để theo dõi luồng thực thi và xác định vị trí cụ thể của bug.

#### **Bước 3: Tập trung vào phần gây ra Fix Bug**

Tìm hiểu rõ ràng về module, class hoặc phần code đang gây ra vấn đề.

Tách và kiểm tra từng chức năng hoặc phần logic để xác định nguyên nhân cụ thể của bug.

#### **Bước 4: Tách nhỏ lỗi và sửa từng phần Fix Bug**

Khi đã xác định được nguyên nhân, thực hiện sửa chữa từng phần nhỏ một cách cẩn thận.

Kiểm tra lại từng phần sau khi sửa đổi để đảm bảo rằng bug đã được khắc phục và không tạo ra vấn đề mới.

#### **Bước 5: Ghi chép và theo dõi quá trình Fix Bug**

Ghi lại các bước đã thực hiện, sửa đổi code và các lưu ý quan trọng về từng phần đã được kiểm tra và fix.

Điều này giúp theo dõi tiến trình và tạo một lịch sử rõ ràng về quá trình fix bug, giúp dễ dàng học hỏi và thực hiện những cải tiến trong tương lai.

### **4. Sử dụng kiến thức Testing**

#### **Bước 1: Xem xét lại Testing**

Đánh giá lại tất cả các testcase đã được thực hiện trong quá trình kiểm thử phần mềm.

Đối chiếu với tài liệu yêu cầu (requirements) và thiết kế để đảm bảo rằng tất cả các kịch bản đã được cover.

#### **Bước 2: Phân tích vấn đề không được xem xét**

Xác định các phần của phần mềm chưa được kiểm tra hoặc không được cover trong quá trình testing trước đó.

Lập danh sách các tính năng, chức năng, hoặc các trường hợp sử dụng không được kiểm tra.

#### **Bước 3: Đánh giá lý do không cover để Fix Bug**

Phân tích liệu có nguyên nhân nào dẫn đến việc không kiểm tra các kịch bản này.

Có thể do hạn chế về thời gian, tài nguyên, hoặc thiếu thông tin về tính năng cụ thể.

#### **Bước 4: Tạo plan để Fix Bug lại**

Xác định cách tiếp cận để bổ sung kiểm thử cho các kịch bản chưa được cover.

Lập lịch kiểm thử lại, bao gồm cả việc tạo testcase mới và kiểm tra lại các kịch bản thiếu sót.

#### **Bước 5: Cải thiện quy trình Testing**

Học từ những lần kiểm thử trước đó để cải thiện quy trình kiểm thử tương lai.

Xem xét cách cải thiện việc xác định và cover các kịch bản kiểm thử để tránh thiếu sót.

### **5. Ghi chép lại quá trình fix bug**

**Ghi chép chi tiết về các thay đổi đã thực hiện để tiện theo dõi và học hỏi:**

- Tạo các ghi chú, comment trong code để mô tả rõ ràng về sự thay đổi.
- Tạo [documentation](https://wiki.matbao.net/docs/) hoặc logs về các bước đã thực hiện trong quá trình fix bug.

# **Quy trình chi tiết để fix bug**

## **Bước 1. Tiếp nhận thông tin về bug**

### **Thu thập thông tin Bug:**

- ***Phản hồi trực tiếp:\*** Thông tin về bug thường đến từ người dùng cuối hoặc nhóm thử nghiệm. Lắng nghe và ghi chép mọi thông tin mà họ cung cấp, bao gồm các bước để tái tạo vấn đề, môi trường sử dụng, và bất kỳ thông tin cụ thể nào liên quan đến lỗi.

![Tìm hiểu về quy trình Fix Bug](https://wiki.matbao.net/wp-content/uploads/2024/01/quy-trinh-fix-bug.png)

- ***Hệ thống bug tracking:\*** Sử dụng các công cụ như Jira, Bugzilla, GitHub Issues, hay các hệ thống tương tự để tạo và quản lý các báo cáo bug. Kiểm tra thông tin được nhập vào hệ thống, đảm bảo rằng nó cung cấp đầy đủ chi tiết về vấn đề để người phụ trách có thể hiểu và xử lý.

### **Kiểm tra thông tin Bug:**

- ***Chi tiết và rõ ràng:\*** Bao gồm các bước cụ thể để tái tạo lỗi, thông tin về môi trường (hệ điều hành, trình duyệt, phiên bản), và bất kỳ thông tin phụ thuộc nào (các thao tác cụ thể, dữ liệu đầu vào, v.v.).
- ***Hình ảnh hoặc video:\*** Nếu có thể, yêu cầu người báo cáo bug cung cấp hình ảnh hoặc video minh họa vấn đề. Điều này giúp người phụ trách bug hiểu rõ hơn về vấn đề và giảm thời gian cần để xác nhận.

## **Bước 2. Xác nhận và tái tạo Fix bug**

### **Xác định tái tạo vấn đề:**

- Ghi chép hoặc yêu cầu người báo cáo bug cung cấp các bước cụ thể mà họ đã thực hiện trước khi gặp phải bug. Điều này bao gồm các hành động, tuần tự thao tác hoặc dữ liệu cụ thể mà họ đã nhập hoặc tương tác với để gây ra bug.
- Sử dụng thông tin này để tái tạo bug trong môi trường phát triển hoặc testing. Quá trình tái tạo này cần chính xác và tương tự như các bước mà người dùng đã thực hiện để gặp phải bug.

### **Xác nhận phạm vi của Bug:**

- Nếu bug được báo cáo từ người dùng, cố gắng xác minh xem liệu bug có xảy ra trên mọi nền tảng, trình duyệt hoặc điều kiện đặc biệt nào khác không.
- Thử tái tạo bug trên nhiều thiết bị, môi trường và điều kiện khác nhau để xác định phạm vi ảnh hưởng của bug.
- Nếu bug chỉ xảy ra trong một số trường hợp cụ thể, hãy xác định các yếu tố đặc biệt (ví dụ: phiên bản phần mềm, cấu hình máy tính, quyền truy cập) mà bug phát sinh để có thể giải quyết vấn đề một cách chính xác.

## **Bước 3. Phân tích và xác định nguyên nhân**

### **Sử dụng công cụ debugging:**

Để fix bug một cách hiệu quả, việc sử dụng các công cụ debugging như Visual Studio Debugger, Chrome DevTools hoặc các công cụ tương tự là rất quan trọng.

- ***Theo dõi log files:\*** Log files cung cấp thông tin quan trọng về hoạt động của ứng dụng. Theo dõi các file log để xác định các thông điệp lỗi, thông tin debug hoặc cảnh báo có liên quan đến bug.
- ***Phân tích log messages:\*** Kiểm tra các thông điệp log để xác định nguyên nhân cụ thể gây ra vấn đề. Làm rõ các thông tin từ log để tìm ra hành động hoặc điều kiện đã dẫn đến bug.
- ***Sử dụng log levels:\*** Sử dụng các cấp độ log (như DEBUG, INFO, ERROR) để tìm kiếm thông tin cần thiết và hạn chế môi trường log để tập trung vào vấn đề cụ thể.
- ***Debugging thông qua code:\*** Sử dụng các công cụ debugging để tạm dừng hoặc theo dõi luồng thực thi của code. Theo dõi giá trị của các biến, hàm gọi và các dòng code để xác định lỗi và điểm mấu chốt gây ra vấn đề.

## **Bước 4. Tiến hành Fix bug**

### **Fix bug:**

- Điều chỉnh code để loại bỏ lỗi cụ thể đã được xác định.
- Thực hiện các thay đổi logic hoặc cú pháp code để sửa vấn đề một cách chính xác và toàn diện.

![Những tiêu chuẩn để tiến hành Fix Bug](https://wiki.matbao.net/wp-content/uploads/2024/01/tieu-chuan-fix-bug.png)

### **Chuẩn mực Fix Bug:**

- Tuân thủ các quy định về cách viết code được đặt ra trong dự án.
- Sử dụng các quy tắc coding conventions được đồng nhất để code trở nên dễ đọc, bảo trì và mở rộng.
- Kiểm tra lại xem các thay đổi đã tuân thủ quy trình kiểm tra code (code review) hay không để đảm bảo chất lượng.

### **Kiểm tra thay đổi khi Fix Bug:**

- Trước khi triển khai, thực hiện kiểm tra và kiểm thử lại để đảm bảo rằng việc sửa đổi không gây ra các vấn đề phụ.
- Đảm bảo rằng các thay đổi không ảnh hưởng đến các phần khác trong hệ thống.

### **Ghi chép và giải thích các thay đổi Fix Bug:**

- Đối với các thay đổi lớn hoặc ảnh hưởng đến nhiều phần của hệ thống, việc ghi chép và giải thích rõ ràng về các thay đổi đã được thực hiện là cần thiết.
- Lưu ý các điểm quan trọng về việc sửa đổi code để những người khác có thể hiểu và duy trì code dễ dàng hơn trong tương lai.

## **Bước 5. Kiểm tra lại sau khi fix bug**

### **Đảm bảo rằng bug đã được fix và không tạo ra vấn đề mới:**

- Xác nhận rằng fix đã được triển khai và áp dụng vào hệ thống.
- Kiểm tra lại bug report để đảm bảo rằng mô tả vấn đề đã được giải quyết đúng cách.

### **Thực hiện kiểm thử tự động hoặc thủ công:**

- Sử dụng các bộ kiểm thử tự động để chạy các [test](https://wiki.matbao.net/test/) case liên quan đến bug đã được fix.
- Nếu không có bộ kiểm thử tự động, thực hiện kiểm thử thủ công để tái tạo vấn đề và đảm bảo rằng bug không còn tồn tại.

### **Kiểm tra xem việc fix bug có tạo ra vấn đề mới không**

- Đôi khi, việc fix bug có thể gây ra các vấn đề mới. Vì vậy, quan trọng để kiểm tra xem có xuất hiện bug mới hoặc có ảnh hưởng đến các phần khác của hệ thống không.
- Thực hiện kiểm thử mở rộng để đảm bảo rằng các thay đổi không gây ra tác động phụ không mong muốn đến hệ thống.

## **Bước 6. Triển khai và theo dõi Fix Bug**

### **Đưa các thay đổi vào production:**

- Tiến hành triển khai các thay đổi đã được kiểm thử và fix bug vào môi trường sản phẩm.
- Sử dụng các công cụ hoặc quy trình phù hợp để đảm bảo việc triển khai được thực hiện một cách an toàn và không ảnh hưởng đến người dùng cuối.

### **Theo dõi hệ thống:**

- Thiết lập các công cụ giám sát và theo dõi để quản lý hiệu suất và sức khỏe của hệ thống sau khi triển khai.
- Tạo cơ chế thông báo tự động để báo cáo về bất kỳ vấn đề nào xuất hiện.
- Thực hiện kiểm tra định kỳ để xác định có bug mới phát sinh sau khi triển khai hay không.

### **Xử lý bug phát sinh sau triển khai:**

- Nếu có bug mới phát hiện sau khi triển khai, tiến hành xác định và fix sự cố này ngay lập tức.
- Ghi chép và phân tích nguyên nhân của bug mới để tránh tái diễn các vấn đề tương tự trong tương lai.

### **Đánh giá:**

- Đánh giá quá trình triển khai để cải thiện các bước tiếp theo.
- Học hỏi từ kinh nghiệm này để tối ưu hóa quy trình triển khai và theo dõi bug.

## **IV. Kết luận**

Fix bug không chỉ là quá trình sửa lỗi, mà còn là cơ hội để cải thiện chất lượng và ổn định của phần mềm. Kỹ năng debugging và quy trình fix bug có thể tối ưu hóa hiệu suất công việc lập trình viên, đồng thời nâng cao trải nghiệm người dùng.