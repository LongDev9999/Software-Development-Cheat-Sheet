# Tổng hợp về chuẩn hóa cơ sở dữ liệu

### Mục tiêu của chuẩn hóa

Loại bỏ dư thừa dữ liệu Loại bỏ update anomaly Loại bỏ insertion anomaly Loại bỏ deletion anomaly

### Các dạng chuẩn hóa dữ liệu

Chuẩn hoá là quá trình tách bảng (phân rã) thành các bảng nhỏ hơn dựa vào các phụ thuộc hàm. Các dạng chuẩn là các chỉ dẫn để thiết kế các bảng trong CSDL.

Mục đích của chuẩn hoá là loại bỏ các dư thừa dữ liệu và các lỗi khi thao tác dư thừa và các lỗi khi thao tác dữ liệu (Insert, Delete, Update). Nhưng chuẩn hoá làm tăng thời gian truy vấn.

**Các dạng chuẩn hoá** (Normal Form) ![img](https://images.viblo.asia/f67dc66b-2714-46bc-88f8-ed3ef41a4864.png) **Dạng chuẩn 1** – 1NF (First Normal Form)

Định nghĩa: Một bảng (quan hệ) được gọi là ở dạng chuẩn 1NF nếu và chỉ nếu toàn bộ các miền giá trị của các cột có mặt trong bảng (quan hệ) đều chỉ chứa các giá trị nguyên tử (nguyên tố)

Ví dụ:

Một bảng (quan hệ) chưa ở 1NF:

| MASV | HOTEN   | DIACHI     | MAMON     | TENMON        | DIEM |
| ---- | ------- | ---------- | --------- | ------------- | ---- |
| A01  | Lê Na   | 12 Thái Hà | M01M02    | CSDLAnh       | 89   |
| A02  | Trần An | 56 Mã Mây  | M01       | CSDL          | 8    |
| A03  | Hà Nam  | 24 Cầu Gỗ  | M01M02M03 | CSDLAnhToán 1 | 689  |

**Dạng chuẩn 2** – 2NF

Định nghĩa Một quan hệ ở dạng chuẩn 2NF nếu quan hệ đó:

- Là 1NF
- Các thuộc tính không khoá phải phụ thuộc hàm đầy đủ vào khoá chính

Ví dụ

- Ví dụ1: Cho quan hệ R = (ABCD) , khoá là AB và tập phụ thuộc hàm F = {AB -> C, AB -> D}là quan hệ đạt chuẩn 2NF.
- Ví dụ2: Cho quan hệ R = (ABCD) , khoá là AB và tập phụ thuộc hàm

F = {AB -> C, AB -> D, B -> DC} là quan hệ không đạt chuẩn 2NF vì có phụ thuộc hàm

B -> DC là phụ thuộc hàm bộ phận (phụ thuộc hàm không đầy đủ) vào khoá. Khi đó ta đưa về dạng chuẩn 2NF như sau:![img](https://images.viblo.asia/cd989226-7237-4333-b0e9-a02bfc067bf7.png)

Nhận xét

Một quan hệ ở dạng chuẩn 2NF nếu thoả mãn 1 trong các đièu kiện sau: Khoá chính chỉ gồm một thuộc tính Bảng không có các thuộc tính không khoá Tất cả các thuộc tính không khoá phụ thuộc hoàn toàn vào tập các thuộc tính khoá chính

**Dạng chuẩn 3** – 3NF

Định nghĩa Một quan hệ ở dạng chuẩn 3NF nếu quan hệ đó:

- Là 2NF
- Các thuộc tính không khoá phải phụ thuộc trực tiếp vào khoá chính

Ví dụ

- Ví dụ1: Cho quan hệ R = (ABCDGH, khoá là AB và tập phụ thuộc hàm F = {AB -> C, AB -> D, AB -> GH} là quan hệ đạt chuẩn 3NF.
- Ví dụ2: Cho quan hệ R = (ABCDGH) , khoá là AB và tập phụ thuộc hàm

F = {AB -> C, AB -> D, AB -> GH, G -> DH} là quan hệ không đạt chuẩn 3NF vì có phụ thuộc hàm G ® DH là phụ thuộc hàm gián tiếp vào khoá. Khi đó ta đưa về dạng chuẩn 3NF như sau:![img](https://images.viblo.asia/b62ec803-e3eb-4397-9e44-93cf88d73074.png)

**Dạng chuẩn BCNF** (Boyce Codd Normal Form)

Định nghĩa Một quan hệ ở dạng chuẩn BCNF nếu quan hệ đó:

- Là 3NF
- Không có thuộc tính khoá mà phụ thuộc hàm vào thuộc tính không khoá.

Ví dụ

- Ví dụ1: Cho quan hệ R = (ABCDGH, khoá là AB và tập phụ thuộc hàm F = {AB -> C, AB -> D, AB -> GH} là quan hệ đạt chuẩn BCNF.
- Ví dụ2: Cho quan hệ R = (ABCDGH) , khoá là AB và tập phụ thuộc hàm

F = {AB -> C, AB -> D, AB -> GH, H -> B} là quan hệ không đạt chuẩn BCNF vì có thuộc tính khoá B phụ thuộc hàm vào thuộc tính không khoá H. Khi đó ta đưa về dạng chuẩn BCNF như sau:![img](https://images.viblo.asia/e61db351-9cd6-42ed-b2d4-2879534b112d.png)

### Phương pháp chuẩn hóa

Nguyên lí cơ bản trong chuẩn hóa CSDL là triệt tiêu dư thừa dữ liệu bằng cách phân rã các quan hệ nhưng không được làm mất thông tin. Tutorial về chuẩn hóa CSDL

**Tutorial 1** - Dùng phương pháp làm phẳng để chuẩn hóa 1NF

Ở đây có một tutorial rất hay về chuẩn hóa CSDL và vì đây là trang công nghệ thông tin chấm tiếng Việt nên tutorial đó cũng đã có bản tiếng Việt cho những bạn không thích tiếng Anh. Mời các bạn thảo luận về chuẩn hóa CSDL ở topic này.

**Tutorial 2** - Dùng phương pháp tách nhóm lặp để chuẩn hóa 1NF

Đây là đề số 4 môn Kĩ thuật phần mềm kì 7 khóa 49 của lớp ĐT12 khoa ĐTVT trường ĐH Bách Khoa HN. Khác với tutorial 1 ở trên dùng phương pháp làm phẳng, tôi dùng phương pháp tách nhóm lặp để đưa về dạng 1NF trước. Để biết về phương pháp tách nhóm lặp, xin xem thêm tutorial 3.

Yêu cầu: thiết kế CSDL quản lí cửa hàng thuốc cần các thông tin sau:

**DB**(Mã hóa đơn, Ngày bán, Tổng tiền Hóa đơn, Mã khách hàng, Tên Khách hàng, Số ĐT Khách hàng, Mã Nhân viên, Số CMT của NV, Tên NV, Địa chỉ NV, Số ĐT Nhân viên (Mã thuốc, Tên thuốc, Công dụng, Ngày SX, Hạn SD, Số lượng, Thành tiền)).

Các phụ thuộc hàm:

- Mã hóa đơn, Mã khách hàng, Mã nhân viên, Mã thuốc, xác định duy nhất 1 hóa đơn, 1 khách hàng, 1 NV, 1 loại thuốc.
- Một hóa đơn có thể có nhiều thuốc nhưng chỉ do một người mua và một nhân viên bán.
- Số CMT của NV-> Tên NV, Địa chỉ NV

**1NF - Loại bỏ nhóm lặp và loại bỏ các thuộc tính tính toán.**

Cần loại 2 thuộc tính tính toán sau: Tổng tiền hóa đơn và thành tiền. Vì đây chính là dữ liệu dư thừa.

1. Hóa đơn(Mã hóa đơn, Ngày bán, Mã khách hàng, Tên Khách hàng, Số ĐT Khách hàng, Mã Nhân viên, Số CMT của NV, Tên NV, Địa chỉ NV, Số ĐT NV)
2. Hóa đơn - Thuốc(Mã hóa đơn, Mã thuốc, Tên thuốc, Công dụng, Ngày SX, Hạn SD, Số lượng)

**2NF - Loại bỏ các phụ thuộc hàm không hoàn toàn vào khóa chính**

Quan hệ Hóa đơn chỉ có khóa đơn nên quan hệ này đã ở 2NF.

Xét quan hệ Hóa đơn - Thuốc : Tên thuốc, Công dụng, Ngày SX, Hạn SD chỉ phụ thuộc vào Mã thuốc mà không phụ thuộc vào toàn khóa nên quan hệ này được tách làm 2 quan hệ sau:

- Hóa đơn - Thuốc(Mã hóa đơn, Mã thuốc, Số lượng)
- Thuốc(Mã thuốc, Tên thuốc, Công dụng, Ngày SX, Hạn SD)

Như vậy, ở dạng 2NF ta có 3 quan hệ:

1. Hóa đơn(Mã hóa đơn, Ngày bán, Mã khách hàng, Tên Khách hàng, Số ĐT Khách hàng, Mã Nhân viên, Số CMT của NV, Tên NV, Địa chỉ NV, Số ĐT NV)
2. Hóa đơn - Thuốc(Mã hóa đơn, Mã thuốc, Số lượng)
3. Thuốc(Mã thuốc, Tên thuốc, Công dụng, Ngày SX, Hạn SD)

**3NF - Loại bỏ các phụ thuộc hàm bắc cầu vào khóa chính**

Ở quan hệ Hóa đơn, ta thấy Tên Khách hàng, Số ĐT Khách hàng chỉ phụ thuộc Mã khách hàng. Số CMT của NV, Tên NV, Địa chỉ NV chỉ phụ thuộc mã nhân viên. Do đó tách quan hệ này thành 3 quan hệ sau:

- Hóa đơn(Mã hóa đơn, Ngày bán, Mã khách hàng, Mã Nhân viên)
- Khách hàng(Mã khách hàng, Tên Khách hàng, Số ĐT Khách hàng)
- Nhân viên(Mã Nhân viên, Số CMT của NV, Tên NV, Địa chỉ NV, Số ĐT NV)

Như vậy, ở 3NF, chúng ta có 5 quan hệ sau:

1. Hóa đơn(Mã hóa đơn, Ngày bán, Mã khách hàng, Mã Nhân viên)
2. Khách hàng(Mã khách hàng, Tên Khách hàng, Số ĐT Khách hàng)
3. Nhân viên(Mã Nhân viên, Số CMT của NV, Tên NV, Địa chỉ NV, Số ĐT NV)
4. Hóa đơn - Thuốc(Mã hóa đơn, Mã thuốc, Số lượng)
5. Thuốc(Mã thuốc, Tên thuốc, Công dụng, Ngày SX, Hạn SD)

**Tutorial 3** - Chuẩn hóa về BCNF Ở đây có giáo trình CSDL (Bằng Tiếng Anh)đề cập về chuẩn hóa rất dễ hiểu. Trình bày khá sâu về anomaly, các dạng chuẩn giải quyết anomaly như thế nào.

Nói chung thì chuẩn hóa CSDL là việc nên biết trong khi học , Vì ngoài thực tế nếu mà đạt được chuẩn càng cao thì CSDL càng bị dư thừa - Tùy theo mục đích sử dụng mà chuẩn hóa hay không ).