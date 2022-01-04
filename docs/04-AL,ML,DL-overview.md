# AI - ML - DL Overview

Thuật ngữ Artificial Intelligence lần đầu tiên được đặt ra vào năm 1956, nhưng vì sao AI ngày nay đã trở nên phổ biến hơn? Đó là do sự gia tăng đáng kể về khối lượng dữ liệu, các thuật toán nâng cao và những cải tiến về khả năng tính toán và lưu trữ.

Trong vài năm qua, AI đã bùng nổ và đặc biệt là từ năm 2015. Phần lớn là do sự sẵn có rộng rãi của GPU giúp xử lý song song nhanh hơn, rẻ hơn và mạnh mẽ hơn. Nó cũng phải thực hiện đồng thời lưu trữ vô hạn thực tế và một luồng dữ liệu của mỗi dải (toàn bộ chuyển động Dữ liệu lớn) – hình ảnh, văn bản, giao dịch, dữ liệu ánh xạ, v.vv..

Dữ liệu không đủ để dự đoán kết quả chính xác. Nhưng bây giờ có sự gia tăng đáng kể về lượng dữ liệu. Các số liệu thống kê cho thấy đến năm 2020, khối lượng dữ liệu lớn tích lũy sẽ tăng từ 4,4 zettabyte lên khoảng 44 zettabyte hoặc 44 trillion (nghìn tỷ) GB dữ liệu.

Giờ đây, chúng tôi thậm chí còn có nhiều thuật toán tiên tiến hơn, khả năng tính toán và lưu trữ cao cấp có thể xử lý lượng lớn dữ liệu như vậy. Do đó, dự kiến ​​sẽ có 70% doanh nghiệp triển khai AI trong vòng 12 tháng tới, tăng so với mức 40% của năm 2016 và 51% của năm 2017

Cách dễ nhất để nghĩ về mối quan hệ của chúng là hình dung chúng như những vòng tròn đồng tâm với AI – ý tưởng xuất hiện đầu tiên – lớn nhất, sau đó là machine learning – nở rộ sau đó, và cuối cùng là deep learning – thúc đẩy sự bùng nổ AI ngày nay – phù hợp với cả hai.

![ALMLDL](../images/ALMLDL-overview01.png)

## I. Artificial Intelligence (AI)
"Trí tuệ nhân tạo là một kỹ thuật cho phép máy móc hoạt động giống con người bằng cách tái tạo hành vi và bản chất của chúng."

Trí tuệ nhân tạo giúp máy móc có thể học hỏi kinh nghiệm của chúng. Máy điều chỉnh phản ứng của chúng dựa trên các đầu vào mới, do đó thực hiện các tác vụ giống như con người bằng cách xử lý một lượng lớn dữ liệu và nhận dạng các mẫu trong đó.

Một số ví dụ về Trí tuệ nhân tạo trong cuộc sống hàng ngày của chúng ta là Siri của Apple, máy tính chơi cờ vua, ô tô tự lái của tesla và nhiều thứ khác. Những ví dụ này dựa trên Deep Learning và xử lý ngôn ngữ tự nhiên.

## II. Machine Learning (ML)

Machine Learning ra đời vào cuối những năm 80 và đầu những năm 90. Nhưng những vấn đề xảy ra với con người khiến Máy học ra đời là gì?

Thống kê (Statistics): Làm thế nào để đào tạo hiệu quả các mô hình phức tạp lớn?

Khoa học máy tính & Trí tuệ nhân tạo (Computer Science & Artificial Intelligence): Làm thế nào để đào tạo các phiên bản mạnh mẽ hơn của hệ thống AI?

Khoa học thần kinh (Neuroscience): Làm thế nào để thiết kế các mô hình hoạt động của não?

Vậy Machine Learning là gì?

“Học máy là một tập hợp con của trí tuệ nhân tạo. Nó cho phép máy học và đưa ra dự đoán dựa trên kinh nghiệm của nó (dữ liệu)"

Hiểu về Học máy với một ví dụ

Giả sử bạn muốn tạo một hệ thống có thể dự đoán cân nặng mong đợi của một người dựa trên chiều cao của nó. Điều đầu tiên bạn làm là thu thập dữ liệu. Hãy để chúng tôi nói rằng đây là cách dữ liệu của bạn trông như thế này:

![ALMLDL](../images/ALMLDL-overview02.png)

Mỗi điểm trên biểu đồ đại diện cho một điểm dữ liệu. Để bắt đầu, chúng ta có thể vẽ một đường đơn giản để dự đoán cân nặng dựa trên chiều cao. Ví dụ, một dòng đơn giản:
```
W = H - 100

W: là trọng lượng (kg)
H: là chiều cao tính bằng (cm)
```
Đường công thức này có thể giúp đưa ra dự đoán. Mục tiêu chính của là giảm chênh lệch giữa giá trị ước tính và giá trị thực tế. Vì vậy, để đạt được nó, chúng tôi cố gắng vẽ một đường thẳng phù hợp với tất cả các điểm khác nhau này và giảm thiểu sai số và làm cho chúng càng nhỏ càng tốt. Giảm sai số hoặc chênh lệch giữa giá trị thực tế và giá trị ước tính sẽ làm tăng độ chính xác.

Hơn nữa, thu thập càng nhiều dữ liệu đưa về thành một điểm, mô hình sẽ càng trở nên tốt hơn. Có thể cải thiện mô hình của mình bằng cách thêm nhiều biến hơn (ví dụ: Giới tính) và tạo các dòng công thức dự đoán khác nhau cho mỗi đặc tính. Sau khi đường được tạo, vì vậy trong tương lai, nếu một dữ liệu mới (ví dụ: chiều cao của một người) được cung cấp cho mô hình, nó sẽ dễ dàng dự đoán dữ liệu cho bạn và sẽ cho biết cân nặng dự đoán của anh ta.

## III. Deep learning (DL)
"Deep Learning là một loại học máy cụ thể đạt được sức mạnh và tính linh hoạt tuyệt vời bằng cách học cách đại diện cho thế giới dưới dạng phân cấp lồng ghép của các khái niệm hoặc sự trừu tượng"

Bạn có thể coi mô hình Deep Learning như một động cơ tên lửa và nhiên liệu của nó là lượng dữ liệu khổng lồ mà chúng tôi cung cấp cho các thuật toán này.

Khái niệm Deep Learning không phải là mới. Nhưng gần đây sự cường điệu của nó đã tăng lên và Deep Learning đang được chú ý nhiều hơn. Lĩnh vực này là một loại máy học đặc biệt được lấy cảm hứng từ chức năng của các tế bào não của chúng ta được gọi là mạng thần kinh (neural) nhân tạo. Nó chỉ đơn giản là lấy các kết nối dữ liệu giữa tất cả các nơron nhân tạo và điều chỉnh chúng theo mẫu dữ liệu. Cần có nhiều nơ-ron hơn nếu kích thước của dữ liệu lớn. Nó tự động có tính năng học ở nhiều cấp độ trừu tượng, do đó cho phép hệ thống học ánh xạ các hàm phức tạp mà không phụ thuộc vào bất kỳ thuật toán cụ thể nào.


Hãy bắt đầu với một ví dụ đơn giản giải thích cách mọi thứ hoạt động ở cấp độ khái niệm.

**Ví dụ 1:**

Hãy thử và hiểu cách bạn nhận ra một hình vuông từ các hình dạng khác.

![ALMLDL](../images/ALMLDL-overview03.png)

Việc đầu tiên là kiểm tra xem có 4 cạnh hay không. Nếu có, kiểm tra thêm, các cạnh được nối với nhau, một lần nữa nếu có, kiểm tra xem nó có vuông góc và cuối cùng tất cả các cạnh của nó bằng nhau hay không ( Đúng!). đây chẳng qua là một khái niệm phân cấp lồng vào nhau.

Những gì chúng tôi đã làm, chúng tôi thực hiện một nhiệm vụ phức tạp là xác định một hình vuông trong trường hợp này và chia nó thành các nhiệm vụ đơn giản hơn. Giờ đây, Deep Learning này cũng làm được điều này nhưng ở quy mô lớn hơn.

**Ví dụ 2:**

Hãy lấy một ví dụ về một máy nhận dạng động vật. Nhiệm vụ của máy là nhận biết hình ảnh cho trước là của mèo hay là chó.

![ALMLDL](../images/ALMLDL-overview04.png)

Điều gì sẽ xảy ra nếu có yêu cầu giải quyết vấn đề tương tự bằng cách sử dụng các khái niệm về học máy, chúng ta sẽ làm gì? Đầu tiên, ta sẽ xác định các đặc điểm như kiểm tra xem con vật có râu hay không, hoặc kiểm tra xem con vật có tai nhọn hay không hoặc đuôi của nó thẳng hay cong.

Tóm lại, chúng tôi sẽ xác định các đặc điểm trên khuôn mặt và để hệ thống xác định các đặc điểm nào quan trọng hơn trong việc phân loại một loài động vật cụ thể.

Bây giờ khi nói đến học sâu. Nó cần phải đi trước một bước. Học sâu tự động tìm ra các tính năng quan trọng để phân loại, so sánh với Học máy nơi chúng tôi phải cung cấp các tính năng theo cách thủ công.


---
## TK
https://www.edureka.co/blog/ai-vs-machine-learning-vs-deep-learning/