# What Is a GPU?

## 1. What Does a GPU Do?

GPU (Graphics Processing Unit), đã trở thành một phần quan trọng trong công nghệ điện toán cho cá nhân và kinh tế số. Được thiết kế để xử lý song song, GPU được sử dụng cho các ứng dụng như xử lý đồ họa, trích xuất video. 
Mọi người thường biết đến GPU với khả năng tối ưu và hỗ trợ đồ họa cho Game. Nhưng hiện nay GPU trở nên phổ biến hơn với việc sử dụng để sáng tạo nội dung (video, hình ảnh) và xu thế hiện nay là Trí tuệ nhân tạo (AI - Artical Intelligence). 

GPU ban đầu chỉ được thiết kết với mục đích tối ưu xử lý đồ họa 3D. Nhưng qua thời gian, GPU trở nên linh hoạt hơn và có thể lập trình, và được cải thiện nhiều về tính năng. Việc này cho phép các lập trình viên đồ họa có thể xây dựng các hiệu ứng hình ảnh thú vị và thực tế hơn với các kỹ thuật nâng cao cho ánh sáng và bóng râm. 
Các Developer đang bắt đầu khai thác năng lực của GPU để tăng tốc các workload trong Tính toán hiệu năng cao ( HPC - High Performance computing ), Deep Learning, ...

2 thập kỉ trước, GPU được sử dụng chính cho tối ưu ứng dụng 3D real-time, như game. Nhưng hiện nay, các nhà khoa học máy tính nhận ra GPU có tiềm năng giải quyết các vấn đề tính toán khó khăn nhất thế giới.


## 2. GPU and CPU: Working Together

GPU và CPU có nhiều điểm chung. Cả hai đều là thành phần tính toán quan trọng, là bộ vi xử lý và đều có khả năng xử lý dữ liệu. Nhưng CPU và GPU lại có kiến trúc và được xây dựng dựa trên mục đích khác nhau.

![CPUvsGPU](../images/GPU-overview01.png)

| | |
|-|-|
|__CPU__| __GPU__ |
| Central Processing Unit | Graphics Processing Unit |
| Several cores | Several cores|
| Low latency | High throughput |
| Good for serial processing | Good for parallel processing |
| Can do a handful of operations at once | Can do thousands of operations at once|

- CPU: Được thiết kế để xử lý đa năng nhiều *loại* tác vụ nhanh chóng (được đo bằng CPU clock speed), nhưng lại bị giới hạn vì các tác vụ phải xử lý lần lượt. CPU chỉ bao gồm một vài lõi với nhiều bộ nhớ đệm có thể xử lý một vài luồng phần mềm cùng một lúc.

- GPU: Khác với CPU, GPU có thể thực thi song song nhiều bộ dữ liệu đẩy vào, được thiết kế với hàng ngàn lõi chạy đồng thời làm cho việc tính toán hiệu quả.

## 3. GPU vs. Graphics Card: What’s the Difference?
Khi mà khái niệm GPU và card đồ họa thường được sử dụng để thay thế cho nhau, nhung vẫn có sự phân biệt tinh tế giữa các khái niệm này.
Giống như bo mạch chủ chứa GPU. Card đồ họa bao gồm cả một bảng bổ trợ kết hợp GPU, bảng này bao gồm các mạch cho phép GPU hoạt động và kết nối tới các phần còn lại của hệ thống.

GPU có 2 dạng cơ bản: integrated và discrete.
- Intergrated GPU không được tách ra thành một card mà thay vào đó là được nhúng, hàn liền vào bo mạch vùng CPU. 
- Discrete GPU là một chip riêng biệt được gắn trên bảng mạch riêng và được lắp vào bảng mạch CPU thông qua PCIe. 

## 4. GPU Architecture


![CPUvsGPU](../images/GPU-overview02.png)


Một GPU bao gồm nhiều Processor Cluster (PC) chứa nhiều Streaming Multiprocessors (SM). Mỗi SM chứa một cache Layer1 và các CUDA cores liên kết với nhau. Thông thường một SM sử dụng cache L1 của mình và cache L2 dùng chung trước khi kéo dữ liệu từ GDDR5 Memory. Kiến trúc này giúp giảm thiểu độ trễ memory.

Nhìn vào số lượng core có thể xác định được khả năng tính toán song song của GPU. Khi kiểm định với card V100 NVIDIA, có chứa 80 SM, mỗi SM chứa 64 cores nên sẽ có tổng 5120 CUDA cores (số CUDA core trên một SM giờ đã được giảm từ 128 xuống còn 64). Một tác vụ cần xử lý sẽ không được schedule vào một core riêng lẻ mà sẽ tương tác với cluster hoặc SM, đó là cách GPU có thể xử lý song song song.

Các CUDA cores này có thể xử lý tính toán cho cả các bài toán Intergers và floating point. CUDA cores trong kiến trúc Amphere có thể xử lý FP64, FP32 hoặc INT trên clock cycle.

---
## 
[1]. https://www.intel.vn/content/www/vn/vi/products/docs/processors/what-is-a-gpu.html

[2]. https://blogs.nvidia.com/blog/2009/12/16/whats-the-difference-between-a-cpu-and-a-gpu/

[3]. https://www.intel.vn/content/www/vn/vi/products/docs/processors/cpu-vs-gpu.html

[4]. https://www.thegioimaychu.vn/tin-tuc/giong-va-khac-nhau-giua-gpu-va-cpu.html

[5]. https://www.omnisci.com/technical-glossary/cpu-vs-gpu

[6]. https://www.techcenturion.com/nvidia-cuda-cores/

[7]. https://core.vmware.com/resource/exploring-gpu-architecture#section4