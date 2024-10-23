# Bài toán tháp Hà Nội và cách giải sử dụng Đệ Quy

![Bài toán tháp Hà Nội và cách giải sử dụng Đệ Quy](https://statics.cdn.200lab.io/2023/09/Blog17.jpg)

Bài toán tháp Hà Nội có lẽ không còn xa lạ với sinh viên CNTT tại Việt Nam. Bài toán này thường xuyên được sử dụng để giảng dạy về đệ quy và lập trình trong các khóa học về Toán học và Khoa học Máy Tính.

Tháp Hà Nội là một bài toán quen thuộc và thú vị trong lĩnh vực toán học và lập trình. Nó mô phỏng việc di chuyển đĩa từ một cọc này sang một cọc khác, tuân theo một số quy tắc nhất định. Bài toán này mang tính logic cao và yêu cầu sử dụng phương pháp đệ quy để giải quyết một cách hiệu quả.

Chắc chắn bạn đã từng nghe về bài toán tháp Hà Nội, một thách thức kinh điển khi nói đến đệ quy trong lập trình. Trong bài viết này, chúng ta sẽ cùng nhau khám phá cách giải quyết bài toán này bằng phương pháp đệ quy, một kỹ thuật mạnh mẽ và linh hoạt mà chúng ta thường gặp trong lập trình.

Hãy cùng bắt đầu và khám phá sự kỳ diệu của đệ quy thông qua bài toán tháp Hà Nội.

(*) Nếu chưa nắm rõ "[Đệ Quy là gì](https://200lab.io/blog/de-quy-la-gi/)?" thì bạn hãy tham khảo bài viết dưới đây của 200Lab nhé.

Đệ Quy là gì? Có bao nhiêu loại Đệ Quy cơ bản?

Đệ quy là một khái niệm rất quan trọng trong cấu trúc dữ liệu và giải thuật nói riêng, và trong ngành khoa học máy tính nói chung. Chúng ta cùng tìm hiểu về đệ quy trong bài viết này nhé.

![img](https://statics.cdn.200lab.io/2023/08/200lab-fav.png)200Lab BlogLương Việt Hải

![img](https://statics.cdn.200lab.io/2023/09/Blog7.png)

## **1. Giới thiệu bài toán tháp Hà Nội**

### **1.1. Lịch sử hình thành bài toán Tower of Hanoi**

Bài toán tháp Hà Nội có nguồn gốc từ một truyền thuyết Ấn Độ và đã được biết đến rộng rãi do nhà toán học người Pháp, Édouard Lucas, giới thiệu vào năm 1883 trong quyển sách "Récréations Mathématiques".

Truyền thuyết kể về một ngôi đền cổ ở Ấn Độ, nơi có ba cây cột đá và 64 chiếc đĩa vàng khác kích cỡ. Các linh mục ở đền thờ phải chuyển toàn bộ các đĩa từ một cột sang cột khác, tuân theo quy tắc không bao giờ đặt đĩa lớn hơn lên đĩa nhỏ hơn. Truyền thuyết nói rằng, khi toàn bộ các đĩa được chuyển đến cột mới, thế giới sẽ kết thúc.

Édouard Lucas đã lấy cảm hứng từ truyền thuyết này để tạo ra bài toán tháp Hà Nội, đặt tên theo tên thủ đô của Việt Nam vào thời đó.

### **1.2. Mô tả bài toán Tháp Hà Nội**

Bài toán tháp Hà Nội được mô tả cụ thể như sau:

Cho 3 cây đinh A, B và C và n chiếc đĩa có kích thước khác nhau. Ban đầu, các chiếc đinh được đặt ở cột A, theo thứ tự lớn nhất ở dưới cùng, nhỏ dần khi đến chiếc đĩa cuối cùng.

Mục tiêu của bài toán là di chuyển toàn bộ chiếc đĩa từ chiếc đinh A sang chiếc đinh C, sử dụng chiếc đinh B làm trung gian, tuân thủ các quy tắc sau:

- Chỉ có 3 đinh để di chuyển, không có chiếc đinh thứ 4 nào.
- Một lần chỉ được di chuyển một đĩa, và chỉ được di chuyển chiếc đĩa nằm trên đỉnh của đinh, không được di chuyển đĩa nằm giữa.
- Một đĩa chỉ có thể được đặt lên một đĩa lớn hơn, tuy nhiên không nhất thiết hai đĩa này phải có kích thước liền kề, tức là đĩa nhỏ nhất có thể nằm trên đĩa lớn nhất.

## **2. Cấu Trúc bài toán tháp Hà Nội**

### **2.1. Các yếu tố trong bài toán tháp Hà Nội**

Bài toán tháp Hà Nội gồm hai yếu tố cơ bản: đĩa và cây đinh (cột). Dưới đây là chi tiết về từng yếu tố:

- **Đĩa**

**Số lượng:** Bài toán có n đĩa, số lượng đĩa có thể thay đổi tùy thuộc vào phiên bản cụ thể của bài toán. Thông thường, để dễ hình dung và giải quyết bài toán, con số lý tưởng là 3.

**Kích thước:** Mỗi đĩa có một kích thước duy nhất và không đĩa nào giống đĩa nào khác. Đĩa được sắp xếp theo thứ tự giảm dần từ trên xuống dưới trên cây đinh ban đầu.

**Di Chuyển:** Chỉ có một đĩa có thể được di chuyển tại một thời điểm, và đĩa chỉ có thể được đặt lên một đĩa lớn hơn hoặc một cây đinh trống.

- **Đinh (Cột)**

**Số lượng**: Có tổng cộng ba cây đinh, thường được gọi là A, B và C.

**Chức Năng:** Cây đinh có chức năng giữ đĩa và hỗ trợ việc di chuyển những chiếc đĩa giữa các.

### 2.2. Quy tắc của bài toán Tower of Hanoi

Dưới đây là quy tắc của bài toán:

1. **Di chuyển một đĩa**: Trong một lần di chuyển, chỉ được phép di chuyển duy nhất chiếc đĩa trên cùng của mỗi đinh.
2. **Thứ tự các đĩa**: Không được đặt đĩa có kích thước lớn hơn lên trên đĩa có kích thướng nhỏ hơn.

### **2.3. Mục tiêu của bài toán Tower of Hanoi**

Bài toán tháp Hà Nội chủ yếu dựa vào sự di chuyển hợp lệ của các đĩa giữa các cây đinh, đồng thời tuân thủ các quy tắc, để đạt được mục tiêu di chuyển tất cả các đĩa từ cây đinh A sang cây đinh C.

## **3. Hướng giải bài toán bài toán tháp Hà Nội**

Để giải được bài toán này, chúng ta có ba bước :

1. Di chuyển n-1 đĩa ở trên cùng ở chiếc đinh ban đầu đến chiếc đinh trung gian.
2. Di chuyển chiếc đĩa lớn nhất ở dưới cùng của chiếc đinh đầu tiên đến chiếc đinh đích
3. Di chuyển n-1 chiếc đĩa ở đinh trung gian sang đinh đích

Dưới đây là cách giải bài toán tháp Hà Nội với số đĩa là hai.

![Giải bài toán tháp Hà Nội với n = 2](https://statics.cdn.200lab.io/2023/09/Screen-Shot-2023-09-25-at-20.29.43.png)Giải bài toán tháp Hà Nội với n = 2

Với số đĩa là 2, công việc của chúng ta rất đơn giản, là di chuyển từng chiếc đĩa một với các bước giải đã nêu trên.

Vậy, với số đĩa lớn hơn 2, làm thế nào để có thể chuyển n-1 chiếc đĩa sang chiếc đinh trung gian.

![Bài toán tháp Hà Nội sẽ khó hơn nếu số đĩa ban đầu lớn hơn 2.](https://statics.cdn.200lab.io/2023/09/Screen-Shot-2023-09-25-at-20.35.15.png)Bài toán tháp Hà Nội sẽ khó hơn nếu số đĩa ban đầu lớn hơn 2.

Từ hình ảnh trên, vấn đề của chúng ta là cần di chuyển cả 2 chiếc đĩa trên cùng ở chiếc đinh A sang chiếc đinh B.
Để có thể di chuyển 2 chiếc đinh này từ A sang B, ta sử dụng lại bài toán đã làm ở trường hợp 2 chiếc đĩa, khi đó, chúng ta có :

- Di chuyển chiếc đĩa trên cùng ở đinh A sang đinh C
- Di chuyển chiếc đĩa thứ hai sang cột B
- Di chuyển chiếc đĩa ở cột C, là chiếc đĩa nhỏ nhất, sang cột B

![img](https://statics.cdn.200lab.io/2023/09/Screen-Shot-2023-09-25-at-21.03.16.png)Khi số lượng đĩa lớn hơn, chung ta cần chia nhỏ bài toán

Các bước tiếp theo diễn ra như sau :

- Di chuyển chiếc đĩa cuối cùng ở đinh A sang đinh C
- Di chuyển chiếc đĩa trên cùng ở đinh B sang đinh A
- Di chuyển chiếc đĩa còn lại ở đinh B sang đinh C
- Cuối cùng, di chuyển chiếc đinh nhỏ nhất ở đinh A sang đinh C

![img](https://statics.cdn.200lab.io/2023/09/Screen-Shot-2023-09-25-at-21.03.51.png)Cách giải còn lại với trường hợp số đĩa bằng 3

Giải quyết bài toán lớn bằng một bài toán nhỏ hơn là biểu hiện rất rõ ràng cho việc chúng ta có thể xử lý bài toán này bằng đệ quy.

Chúng ta sẽ đi sâu hơn về cách giải bài toán tháp Hà Nội ở chương tiếp theo.

## **4. Cách giải quyết bài toán tháp Hà Nội bằng Đệ Quy**

Sau khi biết được các vấn đề và mục tiêu của bài toán, chúng ta có thể phân tích và xử lý bài toán tháp Hà Nội bằng phương pháp đệ quy.

Cách làm đệ quy yêu cầu chúng ta xác định được 2 thứ, **base case** và **recursion case**.

### **4.1. Base case của bài toán tháp Hà Nội**

Với bài toán này, base case chính là trường hợp mà ta di chuyển trực tiếp chiếc đĩa từ đinh ban đầu đến chiếc đinh đích, mà không cần sử dụng đến chiếc đinh trung gian.

Để có thể làm được điều này, số lượng đĩa mà chúng ta cần di chuyển là một chiếc, ứng với n = 1.

Sau đây là đoạn mã viết bằng C++ của base case:

NONE

copy

```none
void TowerOfHanoi(int numberOfDisks, char sourcePeg, char auxiliaryPeg, char targetPeg) {
    if (numberOfDisks == 1) {
        cout << "Move disk 1 from " << sourcePeg << " to " << targetPeg << endl;
        return;
    }
    
    // recursion case
}
```

Với đoạn code trên, khi `numberOfDisks` = 1, ta sẽ dịch chuyển chiếc đĩa đó từ chiếc đĩa nguồn `sourcePeg` đến chiếc đĩa đích `targetPeg`

Sở dĩ chiếc đĩa này luôn là đĩa 1, là đĩa nhỏ nhất, vì chỉ có đĩa 1 mới phù hợp với base case, nghĩa là chúng ta đã di chuyển tất cả các đĩa lớn hơn chiếc đĩa này đến vị trí mong muốn.

Recursion sẽ dừng lại tại thời điểm này vì base case không gọi lại bất kỳ đệ quy nào.

### **4.2. Recursion case của bài toán tháp Hà Nội**

Recursion case là toàn bộ các trường hợp mà số lượng đĩa cần di chuyển lớn hơn một, khi đó chúng ta cần chia nhỏ bài toán, bằng cách liên tục thực hiện đệ quy với số lượng đĩa đã giảm dần sau mỗi lần thực hiện.

Sau mỗi lần thực thi recursion case, chúng ta sẽ tìm cách giảm số lượng đĩa cần di chuyển để chia nhỏ bài toán.

Sau đây là đoạn mã viết bằng C++ của recursion case:

NONE

copy

```none
void TowerOfHanoi(int numberOfDisks, char sourcePeg, char auxiliaryPeg, char targetPeg) {
    // base case
    
    TowerOfHanoi(numberOfDisks - 1, sourcePeg, targetPeg, auxiliaryPeg);
    
    cout << "Move disk " << numberOfDisks << " from " << sourcePeg << " to " << targetPeg << endl;
    
    TowerOfHanoi(numberOfDisks - 1, auxiliaryPeg, sourcePeg, targetPeg);
}
```

Với đoạn code này, chúng ta có 3 bước cần xử lý:

1. Di chuyển n-1 đĩa ở trên cùng ở `sourcePeg` đến `auxiliaryPeg`,
   Mặc dù `auxiliaryPeg` là chiếc đinh trung gian, nhưng để có thể mang được các đĩa này đến `auxiliaryPeg`, ta cần một chiếc đinh trung gian khác, đó chính là chiếc đinh `targetPeg`.
2. Di chuyển chiếc đĩa lớn nhất ở dưới cùng, ứng với `numberOfDisks`, đến chiếc đinh `targetPeg`.
3. Di chuyển `n-1` chiếc đĩa ở `auxiliaryPeg`sang `targetPeg`, và lần này thì chúng ta sử dụng `sourcePeg` làm trung gian nếu số lượng đinh vẫn còn lớn.

Ở câu lệnh 1 và câu lệnh 3, khi số lượng đĩa lớn, chương trình sẽ thực hiện các lời gọi đệ quy nhiều lần để giảm kích thước của bài toán, tức là số lượng đĩa sẽ được giảm dần cho đến khi chỉ còn một đĩa, lúc đó bài toán có thể được giải quyết một cách trực tiếp.

Toàn bộ code để giải bài toán tháp Hà Nội như sau:

NONE

copy

```none
void TowerOfHanoi(int numberOfDisks, char sourcePeg, char auxiliaryPeg, char targetPeg) {
    if (numberOfDisks == 1) {
        cout << "Move disk 1 from " << sourcePeg << " to " << targetPeg << endl;
        return;
    }
    
    TowerOfHanoi(numberOfDisks - 1, sourcePeg, targetPeg, auxiliaryPeg);
    
    cout << "Move disk " << numberOfDisks << " from " << sourcePeg << " to " << targetPeg << endl;
    
    TowerOfHanoi(numberOfDisks - 1, auxiliaryPeg, sourcePeg, targetPeg);
}
```

### **4.3. Phân tích BigO**

Với bài toán tháp Hà Nội, mỗi lần thực hiện chương trình, ta sẽ thực hiện liên tiếp 2 chương trình con nhỏ hơn.

Giả sử ta có số lượng lời gọi hàm đệ quy T(n), ta có thể được mô tả bởi công thức đệ quy sau:

TEXT

copy

```
T(n)=2T(n−1)
```

Khi bạn giải công thức đệ quy trên, bạn sẽ thu được:

TEXT

copy

```
T(n)=2ⁿ−1
```

Do đó, Độ phức tạp thời gian của thuật toán là O(2ⁿ).

Độ phức tạp không gian của đoạn mã này chủ yếu tập trung vào chiều sâu của stack gọi hàm đệ quy. Vì mỗi lời gọi đệ quy tạo ra hai lời gọi đệ quy con, chiều sâu của stack có thể đạt tới n. Do đó, độ phức tạp không gian của đoạn mã này là O(n).

## **5. Kết luận về bài toán tháp Hà Nội**

Bài toán tháp Hà Nội, một bài toán kinh điển trong thuật toán, vẫn tiếp tục là một chủ đề nghiên cứu quan trọng và là một công cụ hữu ích để dạy về đệ quy và giải thuật.

Việc giải bài toán này bằng cách sử dụng đệ quy không chỉ minh họa sức mạnh và độ tinh tế của đệ quy mà còn làm nổi bật tính tự đồng nhất và tái sử dụng code.

Phân tích độ phức tạp của bài toán cho thấy nó có thể trở nên cực kỳ phức tạp với số lượng đĩa tăng lên, với độ phức tạp thời gian là O(2ⁿ) và độ phức tạp không gian là *O*(*n*).

Nhưng mặc dù vậy, việc tìm hiểu về bài toán này có thể mang lại nhiều hiểu biết về thuật toán và lập trình, đặc biệt là đệ quy, giúp phát triển kỹ năng tư duy lập trình và tư duy phân tích vấn đề.

***Tài liệu tham khảo:\***

- [Tower of Hanoi - Wikipedia](https://en.wikipedia.org/wiki/Tower_of_Hanoi?ref=200lab.io)
- [Play Tower Of Hanoi](https://www.mathsisfun.com/games/towerofhanoi.html?ref=200lab.io)
- [Program for Tower of Hanoi Algorithms](https://www.geeksforgeeks.org/c-program-for-tower-of-hanoi/?ref=200lab.io)

Qua việc tìm hiểu và giải quyết bài toán tháp Hà Nội, chúng ta đã được cảm nhận sự phức tạp và thú vị của việc áp dụng phương pháp đệ quy trong lập trình. Đệ quy là một công cụ mạnh mẽ giúp giải quyết các vấn đề phức tạp bằng cách chia nhỏ chúng thành các bài toán nhỏ hơn và kết hợp kết quả từ các bài toán con.

Bài toán tháp Hà Nội là một ví dụ điển hình về cách sử dụng đệ quy một cách hiệu quả. Qua quá trình giải, chúng ta đã thấy rõ cấu trúc và quy luật, từ đó áp dụng phương pháp đệ quy một cách logic và hiệu quả.

Hy vọng rằng việc tìm hiểu về bài toán tháp Hà Nội và cách giải quyết sẽ giúp bạn nâng cao hiểu biết về đệ quy và áp dụng nó trong những bài toán phức tạp hơn trong lập trình.