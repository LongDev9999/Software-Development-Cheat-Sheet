# Các loại mô hình phát triển phần mềm

## Các mô hình phát triển sản phẩm

### 1. Mô hình thác nước (The waterfall morden)

[Mô hình thác nước](https://mdo.com.vn/blog/cac-loai-mo-hinh-phat-trien-phan-mem-ma-ban-nen-biet) hay còn gọi là mô hình vòng đời phát triển hệ thống, là cách tiếp cận đầu tiên để phát triển phần mềm. Quá trình bao gồm việc di chuyển xuống qua các giai đoạn phát triển theo thứ tự như: phân tích, thiết kế, phát triển, thử nghiệm, triển khai và bảo trì. Mỗi giai đoạn được xác định rõ ràng với các sản phẩm và cột mốc cụ thể. Và việc thử nghiệm chỉ được thực hiện khi quá trình phát triển hoàn tất.

![mo-hinh-thac-nuoc-waterfall-morden.png](https://res.cloudinary.com/bsd-assets/image/upload/v1678085498/mo_hinh_thac_nuoc_waterfall_morden_87b45d8caf.png)
**Ưu điểm của mô hình này**

- Phù hợp với các dự án nhỏ hoặc vừa, đơn giản với các yêu cầu xác định rõ ràng và không thay đổi
- Dễ hiểu, dễ sử dụng
- Giúp cho việc phát hiện ra lỗi sớm hơn
  **Nhược điểm:**
- Đây là mô hình tuyến tính tuần tự, nghĩa là bước tiếp theo không thể diễn ra nếu bước trước đó chưa hoàn tất. Không có sự linh hoạt trong mô hình này vì không thể bỏ qua hay chồng chéo các giai đoạn.
- Sự thiếu linh hoạt này làm cho mô hình này tốn nhiều thời gian và chi phí, bên cạnh đó rủi ro sai sót là rất cao
- Gây khó khăn khi có yêu cầu thay đổi của khách hàng
- Không phù hợp với các dự án lớn

### 2. Mô hình chữ V (Mô hình thực tế xác minh)

Đây là mô hình mở rộng dựa trên mô hình thác nước với việc bổ sung kế hoạch thử nghiệm sớm. Việc thử nghiệm được thực hiện song song với quá trình phát triển, cách tổ chức quy trình công việc như vậy hàm ý kiểm soát chất lượng đặc biệt.

![mo-hinh-chu-v-mo-hinh-thuc-te-xac-minh.png](https://res.cloudinary.com/bsd-assets/image/upload/v1678085543/mo_hinh_chu_v_mo_hinh_thuc_te_xac_minh_be210aee9f.png)
**Ưu điểm của mô hình:**

- Việc thử nghiệm cùng với các giai đoạn tương ứng giúp phát hiện lỗi sớm trong đặc tả yêu cầu, mã và kiến trúc trong quá trình phát triển dự án.
- Đơn giản và dễ sử dụng
- Hoạt động tốt với những dự án nhỏ, nơi những yêu cầu được hiểu rõ ràng
- Mang lại cơ hội thành công cao hơn mô hình thác nước
  **Nhược điểm:**
- Giống như mô hình thác nước thì chỉ khi hoàn thành giai đoạn trước mới thực hiện được giai đoạn sau
- Việc điều chỉnh vẫn khá khó khăn, tốn kém và mất nhiều thời gian.

### 3. Mô hình xoắn ốc (Spiral Model)

Mô hình này tập trung vào rủi ro và phân tích rủi ro. Mô hình này gồm 4 giai đoạn: Lập kế hoạch, Phân tích rủi ro, Kỹ thuật và Đánh giá. Đường xoắn ốc cơ bản, bắt đầu từ giai đoạn lập kế hoạch, các yêu cầu được thu thập và đánh giá rủi ro. Mỗi đường xoắn ốc tiếp theo được xây dựng trên đường xoắn ốc cơ bản.
Đây là mô hình có sự tham gia sau rộng của khách hàng. Họ có thể tham gia vào các giai đoạn khám phá và hiểu rõ hơn về mức độ rủi ro ở từng bước phát triển.

![mo-hinh-xoan-oc.png](https://res.cloudinary.com/bsd-assets/image/upload/v1678085622/mo_hinh_xoan_oc_5b39539887.png)
**Ưu điểm của mô hình xoắn ốc:**

- Phân tích được khả năng rủi ro cao, tránh được khả năng rủi ro tăng cường
- Phù hợp với các dự án lớn và quan trọng
- Phê duyệt mạnh mẽ và kiểm tra tài liệu
- Các chức năng bổ sung có thể được thêm vào sau đó một cách dễ dàng
- Giám sát dự án dễ dàng và hiệu quả
  **Nhược điểm:**
- Có thể là mô hình tốn kém khi sử dụng
- Yêu cầu chuyên môn cao, có kỹ năng tốt để quản lý dự án
- Quy trình phức tạp và không thích hợp với các dự án nhỏ, ít rủi ro

### 4. Mô hình mẫu (Prototyping model)

Trong mô hình này tập trung vào việc tăng cường sự hiểu biết của nhóm phát triển về mong muốn/nhu cầu của khách hàng bằng cách tạo ra các nguyên mẫu. Bằng cách tạo một bản sao quy mô nhỏ đang hoạt động của chương trình phần mềm mong muốn, thông tin sai lệch có thể được giải quyết trước khi diễn ra quá trình phát triển đầy đủ.
Nguyên mẫu được phát triển, thử nghiệm và tinh chỉnh theo phản hồi của khách hàng. Sau khi mẫu nguyên được chấp nhận, nhóm bắt đầu phát triển sản phẩm cuối cùng.

![mo-hinh-mau-prototyping-model.png](https://res.cloudinary.com/bsd-assets/image/upload/v1678085684/mo_hinh_mau_prototyping_model_ffcea6314d.png)
**Ưu điểm:**

- Giảm đáng kể số lần lặp lại cần thiết để phát triển phần mềm nhờ những phản hồi sớm của khách hàng
- Tiết kiệm thời gian và tăng độ hài lòng của khách hàng
- Người dùng được tham gia vào qua trình phát triển sản phẩm
- Cải thiện được sản phẩm nhờ biết được những tính năng còn thiếu
  **Nhược điểm của mô hình này:**
- Trên thực tế, phương pháp này có thể làm tăng mức độ phức tạp của hệ thống vì phạm vi của hệ thống có thể mở rộng ra bên ngoài các kế hoạch ban đầu.
- Khi mẫu không truyền tải được hết chức năng mà hệ thống đem lại thì có thể dẫn đến sự thờ ơ của khách hàng ngay cả khi nó chưa chính thức được ra mắt
- Khi mẫu cuối cùng đang được phát triển, không thể thực hiện thêm yêu cầu hoặc thay đổi bất kỳ đối với kế hoạch.

### 5. Mô hình phát triển phương pháp Agile

Phương pháp Agile được phát triển dựa trên 2 phương thức là Iterative (Lặp lại) và Incremental (Tăng dần).
Ngày nay, hơn 70% các tổ chức sử dụng cách tiếp cận Agile này hoặc cách tiếp cận Agile khác trong các dự án CNTT của họ. Nói chung, trọng tâm của Agile là phát triển lặp đi lặp lại, giao tiếp chuyên sâu và phản hồi sớm của khách hàng. Mô hình này được phát triển để cung cấp phần mềm tốt hơn và hiệu quả hơn so với các phương pháp trước đó, bao gồm cả Thác nước, thông qua tập trung vào cộng tác, giao tiếp và thay đổi liên tục.

![mo-hinh-phat-trien-phuong-phap-agile.jpg](https://res.cloudinary.com/bsd-assets/image/upload/v1678085727/mo_hinh_phat_trien_phuong_phap_agile_53c1635b86.jpg)
**Ưu điểm:**

- Sự hài lòng của khách hàng bằng cách cung cấp nhanh chóng, liên tục các phần mềm hữu ích.
- Thời gian cung cấp một phiên bản phần mềm hoạt động mất ít thời gian, thường là vài tuần
- Làm việc với sự cộng tác chặt chẽ trong cả nhóm và với khách hàng
- Thích ứng nhanh chóng với sự thay đổi của hoàn cảnh
  **Nhược điểm:**
- Thiếu sự nhấn mạnh và thiết kế tài liệu cần thiết
- Trong trường hợp một số sản phẩm chuyển giao phần mềm, đặc biệt là những sản phẩm lớn, rất khó để đánh giá nỗ lực cần thiết khi bắt đầu vòng đời phát triển phần mềm.
- việc thiếu kế hoạch chi tiết và cởi mở với những thay đổi gây khó khăn cho việc ước tính chính xác ngân sách, thời gian và con người cần thiết cho dự án.
  **Scrum**
  Scrum có lẽ mô hình Agile phổ biến nhất. Các lần lặp lại ('sprints') thường kéo dài 2-4 tuần và chúng được bắt đầu bằng việc lập kế hoạch kỹ lưỡng và đánh giá nước rút trước đó. Không có thay đổi nào được phép sau khi các hoạt động chạy nước rút đã được xác định.

![scrum.png](https://res.cloudinary.com/bsd-assets/image/upload/v1678085762/scrum_abcfa66b5d.png)