# TẠI SAO LẬP TRÌNH VIÊN NÊN CÓ TƯ DUY VỀ TESTING?

## **Vì sao Dev nên rèn luyện cho mình tư duy Test???**

Đây là câu hỏi mà chắc hẳn rằng không ít người băn khoăn, trăn trở?

Dev: "Đã code sấp mặt rồi lại còn ngồi tư duy Test?"

Tester: "Làm Dev mà có một chút tư duy về Test nữa thì có phải là perfect không?"

Theo sự thống kê và trải nghiệm cho thấy rằng: Mối quan hệ giữa Dev và Test dường như không nhiều chứa hai chữ "hòa bình"

Bên nào rồi cũng cho là mình đúng, mình không sai, luôn mất bình tĩnh và nâng cao "cái tôi".

![img](https://blog.pirago.vn/content/images/2021/10/image.png)

Vì vậy, hãy cùng nhau phân tích xem "Vì sao lập trình viên cần có tư duy về Testing nhé". Chúng ta sẽ cùng đi qua 3 phần:

![img](https://blog.pirago.vn/content/images/2021/10/image-1.png)

**1.Tầm quan trọng của kiểm thử**
Những con số không bao giờ biết nói dối, và để hiểu rõ Test quan trọng như nào thì hãy nhìn qua các con số thống kê sau:

![img](https://blog.pirago.vn/content/images/2021/10/image-2.png)

Những con số thật ấn tượng phải không? Khi đọc qua chắc các bạn đã biết được nó đã ảnh hưởng trực tiếp như thế nào tới cuộc sống, công việc của chúng ta. Vậy tại sao nó lại quan trọng như thế, hãy cùng bước sang phần 2....

**2. Kiểm thử là gì?**

Theo Wikipedia, thì **Kiểm thử phần mềm** (tiếng Anh: **Software testing**) là một cuộc kiểm tra được tiến hành để cung cấp cho các bên liên quan thông tin về chất lượng của [sản phẩm](https://vi.wikipedia.org/wiki/Sản_phẩm) hoặc [dịch vụ](https://vi.wikipedia.org/wiki/Dịch_vụ) được kiểm thử.[[1\]](https://vi.wikipedia.org/wiki/Kiểm_thử_phần_mềm#cite_note-1) Kiểm thử có thể cung cấp cho doanh nghiệp một quan điểm, một cách nhìn độc lập về [phần mềm](https://vi.wikipedia.org/wiki/Phần_mềm) để từ đó cho phép đánh giá và thấu hiểu được những rủi ro trong quá trình [triển khai](https://vi.wikipedia.org/w/index.php?title=Triển_khai&action=edit&redlink=1) phần mềm.

Chính vì thế, kiểm thử dường như đóng vai trò tiên quyết trong việc sản phẩm liệu đã sẵn sàng để đưa đến người dùng hay chưa. Vì vậy chúng ta không thể xem nhẹ việc kiểm thử trong bất kì 1 sản phẩm nào.

Có khá nhiều kỹ thuật để kiểm thử, nhưng hôm nay tớ sẽ giới thiệu tới các bạn 2 kỹ thuật kiểm thử phổ biến được dùng và các bạn dev có thể dễ dàng đọc, hiểu, áp dụng nhanh chóng

**A. Kỹ thuật phân vùng tương đương**

Phân vùng tương đương là phương pháp chia các điều kiện đầu vào thành những vùng tương đương nhau. Tất cả các giá trị trong một vùng tương đương sẽ cho một kết quả đầu ra giống nhau. Vì vậy chúng ta có thể test một giá trị đại diện trong vùng tương đương. Các lớp tương đương được xác định bằng bằng cách lấy mỗi trạng thái đầu vào (thường là 1 câu hay 1 cụm từ trong đặc tả) và phân chia nó thành 2 hay nhiều nhóm.

VÍ DỤ: Form nhập số tầng của tòa nhà bao gồm:

Floor: Text-box

Yêu cầu:

Thiết kế test case sao cho người dùng nhập vào ô text-box chỉ cho nhập ký tự là số với độ dài trong khoảng [0-10]

![img](https://blog.pirago.vn/content/images/2021/10/image-3.png)

(*) Dựa vào yêu cầu bài toán ta có thể có các lớp tương đương(phân vùng) sau:

- Phân vùng 1: Nhập giá trị hợp lệ từ 0=> 10 ký tự
- Phân vùng 2: Nhập giá trị không hợp lệ < 0 ký tự
- Phân vùng 3: Nhập giá trị không hợp lệ > 10 ký tự
- Phân vùng 4: Trường hợp để trống không nhập gì hay nhập ký tự không phải dạng số

Sau khi áp dụng phân vùng tương đương có thể chọn được các ca kiểm thử (test case) sau:

- Case 1: Nhập giá trị từ 0 => 10 (có thể chỉ nhập số 5)=> pass
- Case 2: Nhập giá trị < 0 (có thể chỉ nhập số -5) => hiển thị lỗi
- Case 3: Nhập giá trị > 10 => hiển thị lỗi
- Case 4: Để trống không nhập gì hay nhập ký tự không phải dạng số => hiển thị lỗi

B. Kỹ thuật Phân tích giá trị biên

Kiểm thử giá trị biên là quá trình kiểm thử giữa các đầu cực hạn hoặc ranh giới giữa các phân vùng của các giá trị đầu vào. Với kỹ thuật phân tích giá trị biên, chúng ta dựa vào những nguyên tắc sau:

![img](https://blog.pirago.vn/content/images/2021/10/image-4.png)

Trong đó:

- a-1: giá trị ngay dưới mức tối thiểu
- a: giá trị tối thiểu
- a+1: giá trị ngay trên mức tối thiểu
- b-1: giá trị dưới giá trị tối đa
- b: giá trị tối đa
- b+1: giá trị ngay trên mức tối đa

VÍ DỤ: Hãy xem xét hành vi của text box cho phép đặt Pizza dưới đây:

- Số lượng pizza từ 1 đến 10 được xem là hợp lệ. Một thông báo đặt hàng thành công sẽ hiện lên.
- Trong trường hợp khác, số lượng pizza từ 11 đến 99 sẽ được tính là không hợp lệ vì quá nhiều. Thông báo "Mỗi lần đặt hàng, bạn chỉ có thể đặt tối đa 10 chiếc pizza." sẽ xuất hiện.

Điều kiện kiểm thử sẽ như sau:

1. Bất kỳ Số nào lớn hơn 10 được nhập vào trường Số lượng Pizza (giả sử là 11) được coi là không hợp lệ.
2. Bất kỳ Số nào nhỏ hơn 1, chẳng hạn 0 hoặc số âm, thì nó được coi là không hợp lệ.
3. Các số từ 1 đến 10 được coi là hợp lệ
4. Bất kỳ số có 3 chữ số đều là không hợp lệ.

![img](https://blog.pirago.vn/content/images/2021/10/image-6.png)

Khi áp dụng kỹ thuật phân tích giá trị biên, ta sẽ có các giá trị kiểm thử sau:

0, 1,2,9,10,11,99,100

TRƯỜNG HỢP NÊN SỬ DỤNG PHÂN VÙNG TƯƠNG ĐƯƠNG VÀ KIỂM THỬ BIÊN

1. Phương pháp kiểm thử này được sử dụng để giảm một số lượng rất lớn các trường hợp kiểm thử thành các phần có thể quản lý được.
2. Hướng dẫn rất rõ ràng về việc xác định các trường hợp kiểm thử mà không ảnh hưởng đến hiệu quả của việc kiểm thử.
3. Thích hợp cho các ứng dụng tính toán chuyên sâu với số lượng lớn các biến / đầu vào

**3. Tại sao lập trình viên cần biết Testing**

"Viết phần mềm là đã mệt lắm rồi, lại còn phải biết test nữa"

Đôi khi lập trình viên hay ngửa mặt lên trời than "Trời đã sinh code sao còn sinh bug". Thật ta, còn và bug là đôi bạn đồng hành, ở đâu có code, ở đó có bug :D

Theo thuyết tương đối của cụ Anh-xờ-tanh, càng viết nhiều code, lại càng lòi ra nhiều bug

![img](https://blog.pirago.vn/content/images/2021/10/image-7.png)

Cùng nhìn vào một bài toán dưới đây, bạn sẽ thấy tư duy khác nhau giữa Dev và Tester

![img](https://blog.pirago.vn/content/images/2021/10/image-8.png)

Cả 2 bên đều có chung mục đích là tạo ra sản phẩm hoàn hảo nhất cho khách hàng, nhưng công việc lại hoàn toàn đối nghịch nhau.

Công việc của Developer là phát triển hệ thống, viết code và bỏ bug vào code, còn vai trò của Tester là tìm và lôi đầu những con bug đáng ghét ra cho developer trừng trị.

Developer thì rất tin tưởng code mình hoản hảo không có bug, còn Tester thì chứng minh điều ngược lại bằng cách bới bug ra cho developer sửa.

![img](https://blog.pirago.vn/content/images/2021/10/image-9.png)

Chính vì thế, dưới dây, mình liệt kê lại một số lợi ích khi Dev có tư duy Test và áp dụng vào việc viết code của mình

![img](https://blog.pirago.vn/content/images/2021/10/image-10.png)

1. Tư duy Tester giúp chúng ta nghĩ ra được toàn bộ những case có thể gây ra lỗi cho hệ thống, từ đó nghĩ ra phương pháp giải quyết phù hợp
2. Tư duy Tester cũng sẽ giúp bạn thấu hiểu Tester và dễ giao tiếp với họ hơn
3. Khi viết code, ta sẽ để ý và biết cách tách hệ thống ra từng phần cho dễ test
4. Developer có tư duy Tester sẽ chạy thử code mình viết kĩ lưỡng hơn, tiết kiệm được thời gian cho cả Tester và chính mình
5. Code  viết ra ít có bug hơn, giúp nâng cao chất lượng phần mềm

THÂN ÁI~