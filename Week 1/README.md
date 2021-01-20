## Độ phức tạp thuật toán
### Thuật toán là gì?

Thuật toán là một tập hợp các hướng dẫn để tìm ra giải pháp cho một vấn đề. Nó cung cấp các hoạt động từng bước được thực hiện sẽ đưa bạn từ bất kỳ đầu vào hợp lệ nào cho vấn đề đến đầu ra.

Chúng tôi đã tạo ra các thuật toán, bằng hình thức này hay hình thức khác, trong suốt lớp này.

### Hiệu quả là gì?

Bất cứ khi nào chúng ta tạo ra các thuật toán, chúng ta cần lưu ý rằng chúng chạy trên máy tính và máy tính yêu cầu thời gian và không gian (bộ nhớ) để xử lý mọi lệnh.

Mặc dù hầu hết các thuật toán chúng ta đã viết dường như chạy ngay lập tức, nhưng các thuật toán "tức thì" có thể mất vài phút hoặc vài ngày để chạy nếu có quá nhiều dữ liệu đầu vào để xử lý. Đối với khả năng mở rộng và các hệ thống lớn, điều quan trọng là phải tính đến thời gian và không gian mà một thuật toán sẽ cần để chạy với kích thước đầu vào lớn hơn.

## Common Big O Values


| Input Size (N) |	O(1) |	O(log(N))	 |  O(N)	| O(Nlog(N))	| O(N<sup>2</sup>) |
| :-------------: |	:-------------: |	:-------------:	 | :-------------:	| :-------------:	| :-------------: |
| 1	| 1	 | 0 | 1 |	1 |	1 |
| 8	| 1	|  3	| 8 | 24 | 64  |
| 30	 | 1 | 	~5	 | 30 | 150 | 	900 |
| 500	 | 1 | 	~9	 | 500 | 4500 | 250,000 |
| 1000 | 	1 | 	~10	 | 1000	 | 10,000 | 	1,000,000 |
| 16,000	 | 1	 | ~14	 | 16,000	 | 224,000  | 	256,000,000 |
| 100,000	 | 1	 | ~17	 | 100,000	 | 1,700,000  | 	10,000,000,000 |

#### O(1)

Một thuật toán được coi là  `O(1)`khi : với bất kì giá trị đầu vào thì máy tính tính sẽ thực hiện một lượng công việc cơ bản như nhau để thực hiện thuật toán trên chúng.

O(1): +, -, *, /, %, <, >. ==, ===. (Điều này giả định rằng tất cả các số đều có một số kích thước giới hạn như số 32 bit hoặc số 64 bit.)

Phép gán ( =) return và truy cập một giá trị trong mảng ( arr[4]) hoặc đối tượng ( obj['a']) là các ví dụ khác về các bước được xem xét O(1).
#### O(n)

Để nói một thuật toán là tuyến tính hoặc O(n)có nghĩa là các tài nguyên cần thiết phát triển tỷ lệ thuận với kích thước của đầu vào.

Các thuật toán xử lý mỗi đầu vào ít nhất một lần sẽ mất ít nhất O (n) thời gian. Vòng lặp là một ví dụ phổ biến.

#### O (log (n))

Bất kỳ thuật toán nào cắt kích thước vấn đề thành một nửa ở mỗi bước là logarit hoặc O(log n).

Các thuật toán này mất nhiều thời gian hơn cho các đầu vào lớn hơn, nhưng tốc độ tăng rất chậm so với nhiều khả năng khác.

#### O (nlog(n))
Bạn sẽ thường thấy O(n log(n))trong các thuật toán "chia để trị", cắt một vấn đề thành một nửa, giải quyết cả hai nửa và kết hợp các kết quả thành một giải pháp cuối cùng. Đây O(n log(n))phức tạp nổi tiếng là sự phức tạp thời gian nhanh nhất có thể của thuật toán sắp xếp trên đầu vào không hạn chế.

Tất nhiên, đây cũng sẽ là độ phức tạp về thời gian của một vòng lặp chạy theo n thời gian và O(log(n))hoạt động bên trong.
## Một số cách tính độ phức tạp thuật toán
    - Luật cộng : 
        -Nếu  T1(n) = O(f(n)), T2(n) = O(g(n)), thì T1(n) + T2(n) = O( max {f(n), g(n)} );
- Đánh giá cận : tùy vào input của bài toán mà đưa ra độ phức tạp thuật toán lên dùng


|    complexity	|maximum n |
| :-------------: |	:-------------: |
|Θ(n)	|100 000 000
Θ(nlogn) |	40 000 000
Θ(n<sup>2</sup>)	| 10 000
Θ(n<sup>3</sup>)	|500
Θ(n<sup>4</sup>)	|90
Θ(2<sup>n</sup>)	|20
Θ(N!)	|11
- Luật nhân : Nếu T1(n) = O(f(n)), T2(n) = O(g(n)) và cứ mỗi lần chạy T1 ta đều phải chạy qua O((g(n)) thì độ phức tạp sẽ là T1(n) * T2(n) 


#### Tài liệu tham khảo
- [Topcoder Section 1](https://www.topcoder.com/community/competitive-programming/tutorials/computational-complexity-section-1/)
- [Topcoder Section 2](https://www.topcoder.com/community/competitive-programming/tutorials/computational-complexity-section-2/)
- [VnoiWiki]          (https://vnoi.info/wiki/translate/topcoder/Computational-Complexity-Section-1.md)

