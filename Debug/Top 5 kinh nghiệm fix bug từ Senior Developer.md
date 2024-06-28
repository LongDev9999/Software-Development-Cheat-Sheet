# Top 5 kinh nghiệm fix bug từ Senior Developer

Fix bug muôn đời vẫn là công việc cần làm, sẽ làm của Developer, có là low code platform thì vẫn có bug mà fix, vậy những lập trình viên lâu năm đút túi cho mình kinh nghiệm fix bug gì?



Tất cả sẽ được chia sẻ trong bài viết này. Có tí kinh nghiệm có khi lại hay chứ fix thì ngày nào chả fix.



![kinh nghiệm fix bug từ Senior Developer](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-seniordeveloper.jpg)Văn phong thuần developer, anh em đọc cho vui, tích luỹ được kinh nghiệm gì cho mình thì tích luỹ nha.





## 1. Cố gắng tái hiện bug – Reproduce the Bug



Kinh nghiệm đầu tiên là tái hiện bug, bug vụt qua đời ta nhanh như cờ hó chạy ngoài đồng. Nên ta cần tái hiện.



Tất nhiên dựa vào kinh nghiệm mà anh em [Senior](https://topdev.vn/blog/senior-developer-la-gi/) có thể fix được bug nhanh hơn, nhưng về tái hiện thì chưa chắc. Nếu bug ở trên production, được thực hiện qua một vài trên thao tác UI. Việc tái hiện có thể là tương đương về tốc độ khi [so sánh giữa Senior và Junior](https://topdev.vn/blog/senior-junior-java-dev-dieu-gi-lam-nen-su-khac-biet/).



Tuy nhiên, có một bí mật mà anh em có nhiều kinh nghiệm thường áp dụng để tái hiện bug nhanh nhất có thể. Dưới đây chỉ là một số thông tin ví dụ, tuỳ thuộc vào dự án mà anh em có thể áp dụng để tái hiện nhanh nhất có thể nha!



![kinh nghiệm fix bug từ Senior Developer](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-senior-developer-5.png)Vòng đời thì dài mà ngày nào cũng có. Nguồn ảnh / Source: javatpoint.com



- - Môi trường đang xảy ra bug là gì?. (production, dev hay staging, …)

- - DB đang sử dụng data như nào?

- - Request gửi đi là gì? (capture lại toàn bộ request)

- - Debug đặt đúng chưa (cái này tưởng là ngớ ngẩn nhưng nhiều ông bug trên staging lại debug ở môi trường development)

- - Account đang sử dụng xảy ra bug là account nào?

- - Một số dự án phức tạp còn có thời điểm

- - Các thao tác nào đã thực hiện trước đó để gây ra bug



Sau khi thực hiện đầy đủ các bước, nếu không có gì sai sót thì ôi thôi bug là từ đây mà ra chứ đâu. Tái hiện nhanh đồng nghĩa với việc anh em sẽ có thêm thời gian để fix bug.



[ Top 5 kinh nghiệm fix bug từ Senior Developer](https://topdev.vn/blog/kinh-nghiem-fix-bug-tu-senior-developer/)



## 2. Đánh giá và xác định điểm gây lỗi



Kinh nghiệm fix bug thứ hai là đánh giá và xác định điểm gây ra lỗi. Vậy cụ thể anh em đánh giá như thế nào?



> Sau khi đã tái hiện xong bug, bước thứ hai là đánh giá và xác định chỗ nào gây ra bug. Tất nhiên với các anh em Senior thì đôi khi chỉ cần nhìn mã lỗi hoặc content của lỗi thôi đã đoán ra được bug từ đâu tới. Nhưng đối với anh em còn ít kinh nghiệm thì làm thế nào.



![kinh nghiệm fix bug từ Senior Developer](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-senior-developer-4.jpg)



Cũng không phải quá xì chét (thông thường các anh em mới đều thế). Anh em cứ thử follow một số câu hỏi dưới đây sẽ dễ dàng hơn để tìm ra chỗ gây ra bug:



- - Lỗi này từ đâu mà tới ([Frontend](https://topdev.vn/it-jobs/front-end-kt209) hay [Backend](https://topdev.vn/it-jobs/back-end-kt210), nếu có FE,BE) – Tất nhiên là phỏng đoán.

- - Mã lỗi này thường liên quan tới cái gì – Tất nhiên khúc này không ai có thể cản được anh em google, [Stack overflow](https://topdev.vn/blog/stack-overflow-la-gi-vi-sao-de-quy-lai-de-gay-tran-stack/). Thông thường search tí là ra, nhưng cũng tránh sa đà quá để mà rối.

- - Phần code nào liên quan tới lỗi này (đánh giá sơ bộ dựa trên màn hình, trên nhóm tính năng).



Tại sao phía trên tui lại nhấn mạnh nhiều tới từ sơ bộ, bởi chưa có nhiều kinh nghiệm không thể yêu cầu anh em phải phán đoán chính xác. Việc phán đoán sơ bộ giúp giảm căng thẳng, bình tĩnh từ tốn để tìm ra bug.

***Xem thêm các** **việc làm [tuyển dụng Tester](https://topdev.vn/viec-lam-it/tester-kt78) hấp dẫn tại TopDev***



## 3. Chia để trị – Divide and conquer



> Kinh nghiệm thứ ba cũng là kinh nghiệm xương máu. Chia để trị, nghe như hồi Pháp thuộc mà đúng là như thế thật. Code thì mênh mông bát ngát, nếu mà không chia ra tìm từng phần thì biết tới ngày nào.



Sinh ra cái trò debug cũng thế. Debug cả đống rồi vụt cái bug lướt qua đời ta như một cơn gió. Để thực hiện chia để trị tốt khi tìm và fix bug.



![Divide and conquer](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-senior-developer-3.jpg)



- - Những phần nào không có vấn đề có thể comment

- - Nếu phần trên cần có data cho phần dưới -> có thể hard code hoặc fake data

- - Càng ít code focus tìm lỗi càng tìm lỗi nhanh, anh em nên nhớ

- - Viết được theo kiểu functional programming thì fix nhanh hơn

- - Già đầu hay trẻ trâu thì cũng đều cần chia để trị cho những con bug khóđ

**Chia ra mà trị, chia ra để mà tìm là kinh nghiệm xương máu**. Thường các anh em mới vào hay rén vụ comment hoặc tách rõ phần nào không vấn đề phần nào có vấn đề. Nhưng tin tui đi, anh em đừng ngại, cứ tách bạch ra rồi sẽ tìm được bug nhanh hơn.



## 4. Đánh giá ảnh hưởng



> Kinh nghiệm thứ 4 khi fix bug là đánh giá ảnh hưởng, thường các anh em ít kinh nghiệm quên mất khúc này. Con bug ngồi mò nửa ngày, trằn trọc cả đêm, fix được cái mừng quá nhảy cẫng lên báo deploy, deploy gấp cho bố mà quên đánh giá ảnh hưởng.



Mấy ông có kinh nghiệm thì thường không “háo hức” như thế. Một số câu hỏi cần trả lời trước khi fix xong bug



![Đánh giá ảnh hưởng](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-senior-developer-1.png)



- - Bug này có thể gây ra bug khác không?. Tại sao lại có bug này

- - Những chỗ nào tương tự chỗ này, có thể tiếp tục gây ra bug?

- - Fix được bug này có ảnh hưởng gì tính năng không, cần kiếm tra lại phát cuối



Thường đối với những anh em còn non kinh nghiệm việc đánh giá ảnh hưởng thường rất khó. Có thể task này mình làm nhưng task khác ông kia làm. Tui chả quan tâm, nhưng việc đánh giá ảnh hưởng là rất quan trọng, anh em cần luyện tập để trở thành lập trình viên giỏi. Cái này luyện dần không bao giờ là thừa nha.



## 5. Xác nhận đã fix – verify issue fixed

Cuối cùng cũng là cái hay ho nhất, xác nhận đã fix. Thường rất nhiều anh em bỏ qua mất khúc này. Ồ ze fix xong rồi là fix xong rồi nhưng deploy lên lại cứ lỗi.



![verify issue fixed](https://topdev.vn/blog/wp-content/uploads/2023/11/kinh-nghiem-fix-bug-tu-senior-developer-2.jpg)



Vậy xác nhận đã fix là như thế nào?

- - Còn phần code nào comment không? Fix này lòi kia là do deploy mà quên té comment khúc khác dẫn tới đem lên chạy trật lất.

- - Đã xác nhận fix thật chưa, tái hiện lại tại môi trường gây ra bug, tài khoản gây ra bug

- - Còn chỗ nào giống vậy chưa fix không?

- - Với behavior khác chút xíu thì còn bug không?

Bước này cũng là bước cần thiết để anh em nâng cao trình độ. Nên anh em cố gắng rèn luyện, làm gì cũng cần confirm chắc chắn, bảo fix xong là fix xong chứ không có ơ mà nha.