**[Vietnamese Below]**

## **Practical Back-of-the-Envelope Estimation Tips for System Design**

### **Introduction**

Back-of-the-envelope estimation is a critical skill in system design, especially when evaluating the feasibility of a solution, estimating resource requirements, or planning system capacity. These estimations allow engineers to make informed decisions without diving into overly complex calculations, saving time during the initial design stages.

This approach is not about achieving exact results but rather about developing a solid foundation for realistic expectations and requirements in real-world systems.

### **Key Concepts**

1. **Rounding and Approximation:**
   - In real-world system design, precise calculations are often unnecessary at the early stages. Simplifying calculations helps quickly evaluate the feasibility of a system.
   - **Example:**
     - Instead of solving "99987 ÷ 9.1," round it to "100,000 ÷ 10."
     - This level of approximation is sufficient to determine high-level capacity and resource requirements.

2. **Define and Document Assumptions:**
   - Clearly define and document your assumptions, as they form the basis for your calculations and design.
   - **Example:**
     - Assume a user uploads **2 GB of data per month**, or that a storage system retains logs for **1 year**.

3. **Unit Clarity:**
   - Always specify units when performing estimations to avoid ambiguity.
   - **Example:**
     - Writing "5" without context might lead to confusion—is it 5 KB, 5 MB, or 5 GB? Be explicit: write "5 GB."

4. **Focus on Common Design Metrics:**
   - Frequently used estimations in system design include:
     - **QPS (Query Per Second):** Evaluating system throughput.
     - **Peak QPS:** Planning for high-traffic scenarios.
     - **Storage Capacity:** Estimating data volume for logs, media, or databases.
     - **Network Bandwidth:** Ensuring the network can handle traffic efficiently.
     - **Cache Requirements:** Determining memory size for faster operations.
     - **Scaling:** Estimating the number of servers needed to meet demand.

### **Real-World Applications**

1. **Storage Estimation for Media-Heavy Applications:**
    - **Scenario:** A video-sharing platform stores 1-minute videos uploaded by users. Each video averages 50 MB, and 1 million users upload videos monthly.
    - **Calculation:**
        - Monthly storage: $1 \, \text{million} \times 50 \, \text{MB} = 50 \, \text{TB/month}$

        - Yearly storage: $50 \, \text{TB/month} \times 12 \, \text{months} = 600 \, \text{TB/year}$

2. **QPS Estimation for a Messaging App:**
   - **Scenario:** A messaging platform handles 100 million messages daily.
   - **Calculation:**
     - Average QPS: $QPS = \frac{100 \, \text{million messages}}{24 \, \text{hours} \times 3600 \, \text{seconds}} \approx 1157 \, \text{QPS}$

     - Peak QPS: Assuming peak traffic is 2x the average: $\text{Peak QPS} = 2 \times 1157 = 2314 \, \text{QPS}$


3. **Network Bandwidth Estimation:**
   - **Scenario:** A system streams videos with an average bitrate of 3 Mbps to 10,000 concurrent users.
   - **Calculation:**
     - Total bandwidth required: 

$$
\text{Bandwidth} = 10,000 \times 3 \, \text{Mbps} = 30 \, \text{Gbps}
$$

### **Best Practices for System Design**

1. **Optimize for Scalability:**
   - Use estimations to plan for traffic spikes and ensure the system can scale horizontally by adding more servers or distributing traffic.

2. **Validate Assumptions with Real Data:**
   - After initial estimations, validate the assumptions with production data to refine your design and optimize resource allocation.

3. **Iterative Design:**
   - Use these estimations to create an initial system prototype. Iterate and adjust as you collect more accurate data during testing.

4. **Design for Bottlenecks:**
   - Identify critical system components (e.g., storage, bandwidth, QPS limits) early and ensure they can handle the estimated workload.

### **Conclusion**

Back-of-the-envelope estimation is an essential tool for system designers to quickly and efficiently evaluate system requirements and feasibility. It enables better resource planning, scalability, and bottleneck identification during the early stages of system architecture.

Remember, while these estimations provide a high-level understanding, they are the starting point. Continuous validation and iteration are necessary to ensure the system meets real-world demands.

**Well done! You've taken a significant step in mastering practical system design techniques. Keep building and refining!**

----


## **Mẹo ước tính nhanh trong thiết kế hệ thống thực tế**

### **Giới thiệu**

Ước tính nhanh ("Back-of-the-envelope estimation") là một kỹ năng quan trọng trong thiết kế hệ thống, đặc biệt khi cần đánh giá tính khả thi của giải pháp, ước tính tài nguyên, hoặc lên kế hoạch dung lượng hệ thống. Kỹ thuật này cho phép kỹ sư đưa ra các quyết định sáng suốt mà không cần phải thực hiện các tính toán quá phức tạp, giúp tiết kiệm thời gian trong giai đoạn thiết kế ban đầu.

Phương pháp này không yêu cầu kết quả chính xác tuyệt đối, mà thay vào đó là việc xây dựng nền tảng chắc chắn để đưa ra các yêu cầu và kỳ vọng thực tế cho hệ thống.

### **Các khái niệm chính**

1. **Làm tròn số và xấp xỉ hóa:**
   - Trong thiết kế hệ thống thực tế, các phép tính chính xác không cần thiết ở giai đoạn ban đầu. Đơn giản hóa các phép tính giúp nhanh chóng đánh giá tính khả thi của hệ thống.
   - **Ví dụ:**
     - Thay vì giải bài toán "99987 ÷ 9.1," hãy làm tròn thành "100,000 ÷ 10."
     - Mức xấp xỉ này đủ để đưa ra đánh giá tổng quan về yêu cầu dung lượng và tài nguyên.

2. **Định nghĩa và ghi lại các giả định:**
   - Ghi rõ các giả định bạn đưa ra, vì chúng là cơ sở cho các phép tính và thiết kế của bạn.
   - **Ví dụ:**
     - Giả định rằng một người dùng tải lên **2 GB dữ liệu mỗi tháng**, hoặc rằng hệ thống lưu giữ log trong **1 năm**.

3. **Rõ ràng về đơn vị:**
   - Luôn ghi rõ đơn vị trong các phép tính để tránh nhầm lẫn.
   - **Ví dụ:**
     - Viết "5" mà không có đơn vị có thể gây nhầm lẫn—đó là 5 KB, 5 MB, hay 5 GB? Hãy ghi rõ: "5 GB."

4. **Tập trung vào các chỉ số thiết kế phổ biến:**
   - Một số phép ước tính thường xuyên được sử dụng trong thiết kế hệ thống bao gồm:
     - **QPS (Query Per Second):** Đánh giá khả năng xử lý của hệ thống.
     - **Peak QPS:** Lập kế hoạch cho các kịch bản lưu lượng truy cập cao điểm.
     - **Dung lượng lưu trữ:** Ước tính khối lượng dữ liệu cần lưu trữ (logs, media, database).
     - **Băng thông mạng:** Đảm bảo mạng có khả năng xử lý lưu lượng hiệu quả.
     - **Dung lượng cache:** Ước tính bộ nhớ cần thiết để tăng tốc xử lý.
     - **Mở rộng hệ thống:** Ước tính số lượng máy chủ cần thiết để đáp ứng nhu cầu.

### **Ứng dụng thực tế**

1. **Ước tính lưu trữ cho ứng dụng chứa media:**
   - **Tình huống:** Một nền tảng chia sẻ video lưu trữ video dài 1 phút, mỗi video trung bình 50 MB, và có 1 triệu người dùng tải video lên mỗi tháng.
   - **Tính toán:**
     - Dung lượng hàng tháng: $1 \, \text{triệu} \times 50 \, \text{MB} = 50 \, \text{TB/tháng} $

     - Dung lượng hàng năm: $50 \, \text{TB/tháng} \times 12 \, \text{tháng} = 600 \, \text{TB/năm}$

2. **Ước tính QPS cho ứng dụng nhắn tin:**
   - **Tình huống:** Một nền tảng nhắn tin xử lý 100 triệu tin nhắn mỗi ngày.
   - **Tính toán:**
     - QPS trung bình: $QPS = \frac{100 \, \text{triệu tin nhắn}}{24 \, \text{giờ} \times 3600 \, \text{giây}} \approx 1157 \, \text{QPS}$

     - QPS cao điểm: Giả định lưu lượng cao điểm gấp 2 lần trung bình: $\text{QPS cao điểm} = 2 \times 1157 = 2314 \, \text{QPS}$


3. **Ước tính băng thông mạng:**
   - **Tình huống:** Một hệ thống streaming video cung cấp video với tốc độ trung bình 3 Mbps cho 10,000 người dùng đồng thời.
   - **Tính toán:**
     - Tổng băng thông yêu cầu: 

$$
\text{Băng thông} = 10,000 \times 3 \, \text{Mbps} = 30 \, \text{Gbps}
$$


### **Thực hành tốt nhất trong thiết kế hệ thống**

1. **Tối ưu hóa cho khả năng mở rộng:**
   - Sử dụng các ước tính để lập kế hoạch cho các đợt tăng lưu lượng đột biến, đảm bảo hệ thống có thể mở rộng bằng cách thêm máy chủ hoặc phân phối lưu lượng.

2. **Xác minh giả định bằng dữ liệu thực tế:**
   - Sau các phép ước tính ban đầu, xác minh giả định bằng dữ liệu thực tế để tinh chỉnh thiết kế và tối ưu hóa tài nguyên.

3. **Thiết kế theo hướng lặp:**
   - Sử dụng các phép ước tính để tạo nguyên mẫu hệ thống ban đầu. Thực hiện các vòng lặp để điều chỉnh khi thu thập được dữ liệu chính xác hơn trong quá trình thử nghiệm.

4. **Thiết kế cho các nút thắt cổ chai:**
   - Xác định các thành phần quan trọng của hệ thống (lưu trữ, băng thông, giới hạn QPS) và đảm bảo chúng có thể xử lý được khối lượng công việc dự kiến.

### **Kết luận**

Ước tính nhanh là một công cụ thiết yếu cho các kỹ sư thiết kế hệ thống, giúp nhanh chóng và hiệu quả đánh giá yêu cầu hệ thống và tính khả thi. Phương pháp này giúp lập kế hoạch tài nguyên tốt hơn, cải thiện khả năng mở rộng, và nhận diện các điểm nghẽn trong giai đoạn ban đầu của kiến trúc hệ thống.

Nhớ rằng, các ước tính này chỉ là điểm khởi đầu. Cần liên tục xác minh và lặp lại để đảm bảo hệ thống đáp ứng tốt các nhu cầu thực tế.

**Congratulations on getting this far! Now give yourself a pat on the back. Good job!**
