## **Estimate Twitter QPS and Storage Requirements**

### **Introduction**

This section demonstrates how to estimate the **Query Per Second (QPS)** and storage requirements for a social media platform like Twitter. These calculations are based on assumptions and are not actual Twitter data.

### **Assumptions**

1. **300 million monthly active users (MAU):**
   - The total number of users who access the platform at least once a month.

2. **50% of users use the platform daily:**
   - Out of **300 million MAU**, only **150 million** are daily active users.

3. **Users post an average of 2 tweets per day:**
   - Each user posts **2 tweets/day**.

4. **10% of tweets contain media:**
   - 10% of the tweets include media like images, videos, or attachments.

5. **Data is stored for 5 years:**
   - The system must retain data for **5 years**.

### **QPS Estimation**

1. **Daily Active Users (DAU):**

$$
DAU = 300 \, \text{million} \times 50\% = 150 \, \text{million users/day}.
$$

2. **Total Tweets per Day:**

$$
\text{Total Tweets per Day} = 150 \, \text{million} \times 2 = 300 \, \text{million tweets/day}.
$$

3. **Average QPS:**

$$
QPS = \frac{300 \, \text{million tweets}}{24 \, \text{hours} \times 3600 \, \text{seconds}} \approx 3500 \, \text{QPS}.
$$

4. **Peak QPS:**

   - Assuming peak QPS is **2 times** the average QPS:
   
$$
\text{Peak QPS} = 2 \times 3500 = 7000 \, \text{QPS}.
$$

### **Storage Requirements**

1. **Average Tweet Size:**
   - Each tweet consists of:
     - `tweet_id`: 64 bytes.
     - `text`: 140 bytes.
     - `media`: 1 MB (only 10% of tweets).
   - Average size for tweets with media: **1 MB**.

2. **Daily Media Storage:**

$$
\text{Daily Storage} = 300 \, \text{million tweets/day} \times 10\% \times 1 \, \text{MB} = 30 \, \text{TB/day}.
$$

3. **5-Year Storage:**

$$
\text{5-Year Storage} = 30 \, \text{TB/day} \times 365 \, \text{days/year} \times 5 \, \text{years} \approx 55 \, \text{PB}.
$$

### **Conclusion**

- **System Requirements:**
  - The system must handle **peak QPS of 7000**.
  - **55 PB of storage** is needed for 5 years of media data.
- This exercise illustrates the importance of infrastructure scalability and data management in large-scale distributed systems.

---

## **Ước tính QPS và yêu cầu lưu trữ của Twitter**

### **Giới thiệu**

Phần này minh họa cách ước tính **số lượng truy vấn mỗi giây (QPS)** và yêu cầu lưu trữ cho một nền tảng mạng xã hội như Twitter. Các phép tính này dựa trên các giả định và không phải là dữ liệu thực tế từ Twitter.

### **Giả định**

1. **300 triệu người dùng hoạt động hàng tháng (MAU):**
   - Tổng số người dùng truy cập vào nền tảng ít nhất một lần trong tháng.

2. **50% người dùng sử dụng nền tảng hàng ngày:**
   - Trong số **300 triệu MAU**, chỉ có **150 triệu** là người dùng hoạt động hàng ngày.

3. **Người dùng đăng trung bình 2 tweet mỗi ngày:**
   - Trung bình, mỗi người dùng đăng **2 tweet/ngày**.

4. **10% tweet chứa nội dung đa phương tiện (media):**
   - 10% trong số các tweet có chứa ảnh, video hoặc tệp đính kèm.

5. **Dữ liệu được lưu trữ trong 5 năm:**
   - Hệ thống phải lưu giữ dữ liệu trong **5 năm**.

### **Ước tính QPS**

1. **Người dùng hoạt động hàng ngày (DAU):**

$$
DAU = 300 \, \text{triệu} \times 50\% = 150 \, \text{triệu người dùng/ngày}.
$$

2. **Tổng số tweet mỗi ngày:**

$$
\text{Tổng số tweet/ngày} = 150 \, \text{triệu} \times 2 = 300 \, \text{triệu tweet/ngày}.
$$

3. **QPS trung bình:**

$$
QPS = \frac{300 \, \text{triệu tweet}}{24 \, \text{giờ} \times 3600 \, \text{giây}} \approx 3500 \, \text{QPS}.
$$

4. **QPS cao điểm:**
   - Giả định QPS cao điểm gấp **2 lần QPS trung bình**:

$$
\text{QPS cao điểm} = 2 \times 3500 = 7000 \, \text{QPS}.
$$

### **Yêu cầu lưu trữ**

1. **Kích thước trung bình của tweet:**
   - Một tweet bao gồm:
     - `tweet_id`: 64 bytes.
     - `text`: 140 bytes.
     - `media`: 1 MB (chỉ áp dụng cho 10% số tweet).
   - Tổng kích thước trung bình cho tweet có media: **1 MB**.

2. **Dung lượng lưu trữ mỗi ngày:**

$$
\text{Dung lượng lưu trữ hàng ngày} = 300 \, \text{triệu tweet/ngày} \times 10\% \times 1 \, \text{MB} = 30 \, \text{TB/ngày}.
$$

3. **Dung lượng lưu trữ trong 5 năm:**

$$
\text{Dung lượng 5 năm} = 30 \, \text{TB/ngày} \times 365 \, \text{ngày/năm} \times 5 \, \text{năm} \approx 55 \, \text{PB}.
$$

### **Kết luận**

- **Yêu cầu hệ thống:**
  - Hệ thống phải xử lý được **QPS cao điểm 7000**.
  - **55 PB lưu trữ** cần thiết cho 5 năm dữ liệu đa phương tiện.
- Bài toán này nhấn mạnh tầm quan trọng của khả năng mở rộng cơ sở hạ tầng và quản lý dữ liệu trong các hệ thống phân tán lớn.
