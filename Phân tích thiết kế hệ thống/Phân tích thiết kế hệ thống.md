# Phân tích thiết kế hệ thống thông tin sử dụng biểu đồ UML (Phần 2)

##### Trong [phần 1](https://viblo.asia/Trinh.Pro/posts/PjxMe6yNG4YL) tôi đã giới thiệu với các bạn khái quát về phân tích thiết kế hệ thống thông tin sử dụng biểu đồ UML và 2 dạng biểu đồ ca sử dụng(Use Case Diagram) và biểu đồ lớp (Class Diagram). Trong phần này tôi sẽ tiếp tục giới thiệu tới các bạn một số dạng biểu đồ UML được sử nhiều trong các thiết kế hệ thống

### 1.Biểu đồ tuần tự (Sequence Diagram)

#### 1.1. Giới thiệu biểu đồ tuần tự

Biểu đồ tuần tự là biểu đồ dùng để xác định các trình tự diễn ra sự kiện của một nhóm đối tượng nào đó. Nó miêu tả chi tiết các thông điệp được gửi và nhận giữa các đối tượng đồng thời cũng chú trọng đến việc trình tự về mặt thời gian gửi và nhận các thông điệp đó.

#### 1.2 Các thành phần của biểu đồ tuần tự

- Đối tượng (object or class): biểu diễn bằng các hình chữ nhật

![Untitled(26).png](https://images.viblo.asia/fe845903-6f2b-4bb4-bd66-69e522af792b.png)

- Đường đời đối tượng (Lifelines): biểu diễn bằng các đường gạch rời thẳng đứng bên dưới các đối tượng

![Untitled(8).png](https://images.viblo.asia/576e55c1-b7ec-4ba0-933c-6217bf69dbae.png)

- Thông điệp (Message): biểu diễn bằng các đường mũi tên

Thông điệp được dùng để giao tiếp giữa các đối tượng và lớp. Có nhiều loại thông điệp được định nghĩa ở phần 1.3

![Untitled(9).png](https://images.viblo.asia/53f07977-fc2d-40e6-969a-0b9040bf5a64.png)

- Xử lí bên trong đối tượng (biểu diễn bằng các đoạn hình chữ nhật rỗng nối với các đường đời đối tượng)

![Untitled(10).png](https://images.viblo.asia/31e21ab8-c029-4b52-a08d-7e28eb6bc4a6.png)

#### 1.3 Các loại thông điệp trong biểu đồ tuần tự

- Thông điệp đồng bộ (Synchronous Message)

Thông điệp đồng bộ cần có một request trước hành động tiếp theo.

![Untitled(2).png](https://images.viblo.asia/eacbd1a0-1f31-4ded-9449-a998b4f85798.png)

- Thông điệp không đồng bộ (Asynchronous Message)

Thông điệp không đồng bộ không cần có một request trước hành động tiếp theo.

![Untitled(14).png](https://images.viblo.asia/d4e8ce59-2466-42c0-9c8e-12eb3a64eed3.png)

- Thông điệp chính mình (Self Message)

Là thông điệp mà đối tượng gửi cho chính nó để thực hiện các hàm nội tại.

![Untitled(16).png](https://images.viblo.asia/bcba9ebc-087a-439a-a0ab-0ba4e3a7ad23.png)

- Thông điệp trả lời hoặc trả về (Reply or Return Message)

Là thông điệp trả lời lại khi có request hoặc sau khi kiểm tra tính đúng đắn của một điều kiện nào đó. Ví dụ thông điệp loại này như tin nhắn trả về là success hoặc fail

![Untitled(15).png](https://images.viblo.asia/3bcad42c-e00e-4bbf-bcb4-348769354b62.png)

- Thông điệp tạo mới (Create Message)

Là thông điệp được trả về khi tạo mới một đối tượng.

![Untitled(17).png](https://images.viblo.asia//9b45434e-fe70-4f26-a26e-842085449e50.png)

- Thông điệp xóa (Delete Message) Là thông điệp được trả về khi xóa một đối tượng.

![Untitled(18).png](https://images.viblo.asia/79309860-2782-4e92-a351-d8ab2021e988.png)

#### 1.4 Ví dụ

- VD1: Sơ đồ tuần tự của chức năng đăng nhập.Xem xét đối tượng tài khoản sau đây

![Untitled(22).png](https://images.viblo.asia/2c801130-b1ac-4e17-a910-40762c58e5a4.png)

Trong sơ đồ trên có 3 đối tượng là : người dùng, hệ thống và tài khoản. Luồng xử lí của chức năng đăng nhập có thể diễn giải như sau.

1. Người dùng gửi yêu cầu đăng nhập đến hệ thống.
2. Hệ thống yêu cầu người dùng nhập email và mật khẩu.
3. Người dùng nhập email và mật khẩu.
4. Hệ thống gửi email và mật khẩu của người dùng để kiểm tra.
5. Tài khỏan kiểm tra thông tin email và password có đúng hay không.
6. Tài khoản trả về kết qủa kiểm tra cho hệ thống.
7. Hệ thống trả về thông báo cho người dùng.

### 2.Biểu đồ trạng thái (State Diagram)

#### 2.1. Giới thiệu về biểu đồ trạng thái

Biểu đồ trạng thái là dạng biểu đồ mô tả các trạng thái có thể có và sự chuyển đổi giữa các trạng thái đó khi có các sự kiện tác động của một đối tượng.

Đối với các đối tượng có nhiều trạng thái thì biểu đồ trạng thái là sự lựa chọn tốt nhất giúp chúng ta có thể hiểu rõ hơn về hệ thống.

#### 2.2. Các thành phần của biểu đồ trạng thái

- Trạng thái bắt đầu: (Initial State)

![Untitled.png](https://images.viblo.asia/4e28467b-de3f-414b-afed-4cd0cf209293.png)

- Trạng thái kết thúc: (Final State)

![Untitled(1).png](https://images.viblo.asia/fb72deda-1d56-427e-abb8-4cac505c3614.png)

Trong biểu đồ, đường mũi tên chỉ ra sự biến đổi từ một trạng thái sang trạng thái khác.

- Sự kiện (Event) hoặc Chuyển đổi (Transition)

![Untitled(2).png](https://images.viblo.asia/c5627259-a7d6-46e9-b9f1-c5623814a214.png)

- Trạng thái đối tượng (State)

![Untitled(3).png](https://images.viblo.asia/24fb8c34-535f-41e4-84f1-a92eb5e18120.png)

#### 2.3.Ví dụ

Biểu đồ trạng thái thể hiện lớp Sach trong một hệ thống quản lí thư viện điện tử:

![Untitled(25).png](https://images.viblo.asia/b1521b91-663d-4f40-8273-41567cb2c00f.png)

Biểu đồ trạng thái của lớp Sach trên có thể diễn tả lại như sau: Biểu đồ có 5 trạng thái thái chính là sẵn sàng cho mượn, đã có người mượn, hết hạn lưu hành, đã mượn, mất. và hai trạng thái phụ là trạng thái khởi tạo và trạng thái kết thúc.

1. Sách khởi tạo ở trạng thái "sẵn sàng cho mượn" .
2. Sách chuyển từ trạng thái "sẵn sàng cho mượn" sang trạng thái "Đã mượn" khi có người mượn sách.
3. Sách chuyển từ trạng thái "sẵn sàng cho mượn" sang trạng thái "Hết hạn lưu hành" khi có quyết định hết hạn lưu hành.
4. Sách "đã có người mượn" chuyển sang trạng thái "Hết hạn lưu hành" khi có quyết định hết hạn lưu hành.
5. Sách chuyển từ trạng thái "hết hạn lưu hành" sang trạng thái "lưu trữ" khi có quyết định lưu trữ .
6. Sách chuyển từ trạng thái "đã có người mượn" sang trạng thái "mất" khi làm mất.
7. Sách chuyển từ trạng thái "đã có người mượn" sang trạng thái "sẵn sàng cho mượn" khi trả sách.

### 3. Biểu đồ hoạt động (Activity Diagram)

#### 3.1. Giới thiệu biểu đồ hoạt động

Biểu đồ hoạt động là biểu đồ mô tả các bước thực hiện, các hành động, các nút quyết định và điều kiện rẽ nhánh để điều khiển luồng thực hiện của hệ thống. Đối với những luồng thực thi có nhiều tiến trình chạy song song thì biểu đồ hoạt động là sự lựa chọn tối ưu cho việc thể hiện. Biểu đồ hoạt động khá giống với biểu đồ trạng thái ở tập các kí hiệu nên rất dễ gây nhầm lẫn. Khi vẽ chúng ta cần phải xác định rõ điểm khác nhau giữa hai dạng biểu đồ này là biểu đồ hoạt động tập trung mô tả các hoạt động và kết qủa thu được từ việc thay đổi trạng thái của đối tượng còn biểu đồ trạng thái chỉ mô tả tập tất cả các trạng thái của một đối tượng và những sự kiện dẫn tới sự thay đổi qua lại giữa các trạng thái đó.

#### 3.2 Các thành phần của biểu đồ hoạt động

- Trạng thái khởi tạo hoặc điểm bắt đầu (Initial State or Start Point)

![Untitled.png](https://images.viblo.asia/9ab04dff-1a3e-45bc-8679-9bd05fd2e1fd.png)

- Hoạt động hoặc trạng thái hoạt động (Activity or Action State)

![Untitled(30).png](https://images.viblo.asia/b91cefeb-85ef-4c3e-a3aa-97973a9d8dd2.png)

Hoạt động và sự chuyển đổi hoạt động được ký hiệu và cách sử dụng hoàn toàn giống như trạng thái trong biểu đồ trạng thái đã nêu ở trên.

- Nút quyết định và rẽ nhánh

Nút rẽ nhánh trong biểu đồ hoạt động được kí hiệu bằng hình thoi màu trắng.

![Untitled(32).png](https://images.viblo.asia/f5396290-ffbf-4e0f-8f3f-3b1766a7d42e.png)

- Thanh tương tranh hay thanh đồng bộ

Có thể có nhiều luồng hành động được bắt đầu thực hiện hay kết thúc đồng thời trong hệ thống.

Thanh đồng bộ kết hợp:

![Untitled(7).png](https://images.viblo.asia/0e853cfb-6092-4ad2-bc80-5416df75907a.png)

Thanh đồng bộ chia nhánh:

![Untitled(6).png](https://images.viblo.asia/c518484d-ffdd-47eb-a8ac-ac0278e9ea6d.png)

- Cạnh gián đoạn (Interrupting Edge)

![Untitled(29).png](https://images.viblo.asia/e9ac5753-34af-4c2c-af3b-0e85da3cf7ad.png)

- Luồng hoạt động (Action Folow)

![Untitled(14).png](https://images.viblo.asia/73b5adfe-24b6-422f-a5ce-1db349134508.png)

- Phân làn (Swimlanes)

Phân làn trong biểu đồ sử dụng là những đường nét đứt thẳng đứng theo các đối tượng. Phần kí hiệu này thường được sử dụng để làm rõ luồng hoạt động của các đối tượng riêng biệt.

- Thời gian sự kiện (Time Event)

![Untitled(31).png](https://images.viblo.asia/fff7c6f2-7a2f-43d8-81fd-46dc80ce7f17.png)

- Gửi và nhận tín hiệu (Sent and Received Signals)

![Untitled(27).png](https://images.viblo.asia/2fe1abf6-0526-47b1-a6e4-b8c3538b8943.png)

- Trạng thái kết thúc hoặc điểm cuối (Final State or End Point)

![Untitled(21).png](https://images.viblo.asia/ea5c20d0-c428-4f52-be3e-634273592671.png)

### 3.3 Ví dụ

- VD1:Biểu đồ hoạt động rút tiền tại cây ATM:

![Untitled(5).png](https://images.viblo.asia/854fddf3-1449-4ec0-8f42-06b4187320f8.png)

Như trên hình vẽ ta thấy có ba hoạt động cùng diễn ra là xác nhận thẻ, xác nhận mã số PIN và xác nhận số tiền rút.Chỉ khi sử dụng biểu đồ hoạt động mới có thể miêu tả được các hoạt động song song như vậy.

- VD2: Thêm một ví dụ nữa để chúng ta hiểu hơn về biểu đồ hoạt động với các hành động được phân làn.

Biểu đồ hoạt động thể hiện một qúa trình đặt hàng.

![Untitled(33).png](https://images.viblo.asia/7f42dd9d-3d96-4d82-bcdf-8e3468782f5f.png)

### 4.Lời kết và tài liệu tham khảo

Như vậy tôi đã giới thiệu xong với các bạn 5 dạng biểu đồ cơ bản rất hay được sử dụng trong các tài liệu phân tích thiết kế hệ thống thông tin lớn:

- Biểu đồ ca sử dụng (Usecase Diagram)
- Biểu đồ lớp (Class Diagram)
- Biểu đồ tuần tự (Sequence Diagram)
- Biểu đồ trạng thái (State Diagram)
- Biểu đồ hoạt động (Activity Diagram)

Những tài liệu này rất quan trọng và là một quy chuẩn chung cho tất cả các lập trình viên và nhà phát triển hệ thống. Nó giúp cho công việc mô tả các hệ thống lớn trong qúa trình phát triển và bảo trì sau này một cách chuyên nghiệp.

Các bạn có thể xem các qui định chuẩn trong thiết kế biểu đồ UML tại đây: