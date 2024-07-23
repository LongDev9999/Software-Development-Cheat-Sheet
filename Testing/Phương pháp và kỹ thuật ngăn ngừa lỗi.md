# Phương pháp và kỹ thuật ngăn ngừa lỗi

**1. Cách tiếp cận ngăn ngừa lỗi hiệu quả và một cái nhìn cẩn trọng**

Quality Assurance là một từ được dùng khá nhiều ngày nay, để chỉ đến nhóm kiểm thử trong dự án IT.

Về mặt kỹ thuật, hoạt động QA không chỉ tập trung vào việc xác định lỗi (defect identification – tìm thấy sau khi lỗi xảy ra – đơn giản là kiểm thử – Testing hay quản lý chất lượng Quality Control – QC), mà còn bao gồm cả việc ngăn ngừa lỗi (đảm bảo lỗi không thể xảy ra ngay từ đầu hoặc lỗi được phát hiện và chỉnh sửa trước khi xảy ra trên sản phẩm phần mềm).

Một phương trình tương đương có thể viết như sau:

**QA = QC (xác định lỗi) + Ngăn ngừa lỗi**

Mặc dù có vẻ đơn giản, nhưng khó để xác định được bằng cách nào hay các công việc cần tiến hành để ngăn ngửa lỗi chính xác là gì.
Và một sự thật là, tìm thấy lỗi trong khi thực thi kiểm thử hay sau khi đưa sản phẩm ra thị trường thì tốn kém hơn tìm và chỉnh sửa trước đó; thêm vào là khả năng mất lòng tin của khách hàng. Do đó, ngăn ngửa lỗi càng sớm sẽ càng tốt. Bên cạnh đó, ngăn ngừa lỗi cũng giúp cho công ty được chứng nhận CMMI với thứ hạng cao.

**2. Ngăn ngừa lỗi**

**Ngăn ngừa lỗi là một bước hay một hoạt động quan trọng trong quá trình phát triển phần mềm,** và có thể được chỉ rõ ở các mục dưới đây, chiếm một phần trong các nhiệm vụ kiểm thử của nhóm kiểm thử.

Về cơ bản, việc ngăn ngừa lỗi cho những kỹ sư kiểm thử trong từng giai đoạn sẽ là:

**🌺 Đánh giá các yêu cầu chức năng – Requirement Specification Review:**

Sau khi hiểu rõ các yêu cầu của khách hàng, kỹ sư kiểm thử cần liệt kê một bản ý chính của yêu cầu cho bản thân.

Một bản đánh giá chung là quan trọng ở bước này – đầu tiên, đánh giá nên được làm chung với cả nhóm, sau đó là đánh giá chung với bên ngoài nhóm (bởi nhóm phát triển – dev hay nhóm phân tích chức năng – BA hay khách hàng) để đảm bảo toàn bộ quan điểm, ý kiến, mối quan ngại đều được thống nhất.

**🌺 Đánh giá thiết kế**

Giai đoạn Thiết kế có thể xem như là một giai đoạn phân loại chiến lược và kiểm tra đầu-cuối sẽ đảm bảo nhóm QA hiểu rõ ưu khuyết điểm của từng chiến lược.

Cách đánh giá này sẽ giúp tìm ra bất kỳ vấn đề tương ứng với từng chiến lược và chỉnh sửa, thay đổi nó trước khi tiến đến giai đoạn kế tiếp. Nó có thể được xem như việc nghiên cứu tính khả thi của chiến lược.

**🌺 Đánh giá mã nguồn**

Không có nhiều việc cho kỹ sư kiểm thử ở giai đoạn này, nhưng việc đánh giá cũng nên có ở đây. Kỹ sư phát triển kiểm tra các mã, kiểm tra đầu-cuối và đánh giá trước khi tiến hành kiểm thử đơn vị, kiểm thử tích hợp ứng dụng.

**3. Phương pháp và kỹ thuật ngăn ngừa lỗi**

Một vài phương pháp truyền thống và phổ thông được dùng từ lâu cho việc ngăn ngừa lỗi được liệt kê:

**Đánh giá và kiểm tra:** Phương pháp này bao gồm việc đánh giá bởi từng thành viên trong nhóm (tự-đánh-giá), đánh giá nhóm và kiểm tra trên toàn bộ tài liệu, sản phẩm.

**Kiểm tra đầu-cuối (Walkthrough)**: Phương pháp này có thể gần giống với Đánh giá, nhưng nó thiên về việc so sánh hệ thống từ khi là nguyên mẫu (prototype), khi mà ý tưởng mới hình thành, so với mức độ chính xác của hệ thống.

**Tài liệu hóa lỗi:** Phương pháp này cung cấp những thông tin quan trọng và các thông số mà có thể dùng để hỗ trợ việc phân tích lỗi.

**Phân tích nguyên nhân (Root cause analysis):** Phân tích nguyên nhân bao gồm hai cách tiếp cận chính:

**🌺** Phân tích Pareto – Nguyên lý 20/80

Phân tích Pareto là một kỹ thuật chuẩn và đơn giản giúp đánh giá mức độ của các giải pháp với các tác động tối ưu. Nó cho rằng 80% vấn đề đến từ 20% nguyên nhân.

Do đó, một khi vấn để được xác định và phân loại theo tần suất và một phân tích dựa vào thống kê chi tiết sẽ chỉ ra 20% lượng nguyên nhân gây ra 80% vấn đề. Bằng cách đơn giản là tập trung và loại bỏ vào 20% nguyên nhân, kết quả sẽ được đảm bảo trong khi tối ưu số lượng công việc.

**🌺** Phân tích xương cá

Hay cũng được gọi là phân tích Ishikawa, là một kỹ thuật phân tích nguyên nhân một cách trực quan. Không dùng đến kỹ thuật thống kê tham gia vào quá trình phân tích mà dựa vào phân tích (brainstorming) của cả nhóm. Lược đồ dưới đây mô tả chi tiết kỹ thuật này:

> **Vấn đề sẽ được viết ở ngoài cùng bên phải, và một đường thẳng nối từ đó ra, liệt kê từng nguyên nhân gây ra vấn đề.  Nhánh nào có nhiều nhánh con/nguyên nhân là vấn đề nghiêm trọng nhất và sẽ được tập trung để loại bỏ. Kỹ thuật này đôi khi còn được coi là kỹ thuật phân tích nguyên nhân và kết quả.**
>
> *Ví dụ* **sử dụng biểu đồ Ishikawa của một quán cà phê** **để tìm ra nguyên nhân tại sao khách hàng phản hồi cà phê của quán không ngon.**
>
> ![img](https://blog.pirago.vn/content/images/2022/07/image-12.png)
>
> **4. Thứ hạng TMM và kiểm soát lỗi bởi tổ chức kiểm thử**
>
> TTM (Testing Maturity Model -Mô hình phát triển kiểm thử) được phát triển từ CMM (Capability Maturity Model – mô hình phát triển khả năng)
>
> Ngăn ngửa lỗi cần đến sự tham gia và đóng góp của nhiều thành viên ở từng giai đoạn khác nhau, đó cũng là lý do để nó là một yếu tố nổi bật trong đánh giá TMM thứ hạng 5; Nếu một lỗi xuất hiện thường xuyên trong bất kỳ một bài kiểm thử hay chức năng, tổ chức kiểm thử có thể lập môt nhóm thành viên để phân tích lỗi và phát triển một kế hoạch với các hành động để giải quyết vấn đề/lỗi đó.
>
> Vài lợi ích của việc ngăn ngửa lỗi:
>
> \-  Thành viên trong nhóm sẽ có động lực và tỉnh táo để làm việc
> \-  Sự hài lòng của khách hàng
> \-  Tăng độ tin cậy, khả năng quản lý và tính dự báo
> \-  Tăng cường khả năng cải tiến quá trình
>
> **5.Trách nhiệm và vai trò nhóm trong ngăn ngừa lỗi**
>
> Có ba nhóm chính tham gia vào quá trình ngăn ngửa lỗi
>
> **🌺 Quản lý**
>
> \-  Để đảm bảo cho sự thành công của viện ngăn ngừa lỗi không thể thiếu sự hỗ trợ mạnh mẽ từ ban quản lý
> \-  Sự hỗ trợ có thể la nhân sự, tài nguyên, đào tạo và công cụ dành cho việc tiến hành kế hoạch một cách thuận lợi
> \-  Có chính sách thích hợp và thay đổi văn hóa nếu cần thiết
> \-  Thúc đẩy các cuộc thảo luận, phân bổ các danh sách lỗi và những thay đổi trong quá trình làm việc
>
> **🌺** Kỹ sư kiểm thử
>
> \-  Bảo trì cơ sở sữ liệu về lỗi, đảm bảo tính chính xác của dữ liệu
> \-  Thông tin và dữ liệu về lỗi phải được cập nhật liên tục theo thời gian thực
> \-  Lên kế hoạch triển khai những thay đổi nếu có từ ban quản lý
>
> **🌺** Khách hàng
>
> \-  Vai trò của khách hàng khá nhỏ và hạn chế nhưng sự quan tâm đối với chất lượng của họ là rất quan trọng
>
> **6. Kết luận**
>
> Ngăn ngừa lỗi đóng một vai trò chủ yếu và quan trọng trong chu trình phát triển phần mềm. Nó giúp việc quản lý chất lượng của sản phẩm phần mềm với cách thức “sớm nhất và rẻ nhất” với các phương pháp và kỹ thuật được bàn ở trên.
>
> Nó đảm bảo các vấn đề sẽ được giải quyết sớm mà không để xảy ra trên ứng dụng. Nó đánh giá việc tìm ra nguyên nhân chính là việc căn bản nhất trong quá trình xác định và giải quyết vấn đề.
>
> Duy trì chất lượng của phần mềm là nhiệm vụ của nhóm quản lý và toàn bộ nhóm kiểm thử, bao gồm cả trưởng nhóm, khách hàng và từng thành viên trong nhóm.
>
> 
>
> Reference: https://vntesters.com/defect-prevention/