**[Vietnamese Below]**
## **Availability Numbers**

### **High Availability (HA)**

**High Availability** refers to the ability of a system to remain operational for a long period without downtime. High availability is typically expressed as a percentage, where **100%** means zero downtime. In practice, most services achieve availability between **99% and 100%**.


### **Service Level Agreement (SLA)**

**Service Level Agreement (SLA)** is a formal contract between a service provider and its customer, defining the agreed level of uptime the service must deliver. 

- Leading cloud providers like **Amazon**, **Google**, and **Microsoft** set their SLA levels at **99.9% or higher**.
- Uptime is traditionally expressed in terms of "nines." The more nines, the higher the availability and the lower the downtime.


### **Table of Downtime vs. Availability**

| **Availability %** | **Downtime per day**  | **Downtime per year**  |
|---------------------|-----------------------|-------------------------|
| **99%**            | 14.40 minutes         | 3.65 days              |
| **99.9%**          | 1.44 minutes          | 8.77 hours             |
| **99.99%**         | 8.64 seconds          | 52.60 minutes          |
| **99.999%**        | 864.00 milliseconds   | 5.26 minutes           |
| **99.9999%**       | 86.40 milliseconds    | 31.56 seconds          |


### **Analysis and Practical Examples**

1. **Decreasing Downtime with Higher Availability:**
   - At **99% availability**, the system may experience **14.40 minutes of downtime per day**, equivalent to **3.65 days per year**.
   - At **99.999% availability** ("five nines"), downtime is reduced to only **864 milliseconds per day**, or around **5.26 minutes per year**.

2. **Use Cases for Different Availability Levels:**
   - **99%:** Suitable for non-critical systems, such as personal websites or internal tools.
   - **99.9%:** Appropriate for e-commerce applications where downtime impacts revenue but is manageable.
   - **99.99% and above:** Required for critical systems, such as healthcare, financial services, and large-scale cloud platforms, where downtime can have severe consequences.


### **Real-World Examples**

1. **E-commerce Website:**
   - An online store with **99.9% availability** could face **1.44 minutes of downtime daily**. During this time, customers cannot make purchases.

2. **Online Banking:**
   - A bank achieving **99.999% availability** ensures maximum yearly downtime of only **5.26 minutes**, maintaining seamless transactions for its customers.

3. **IoT Traffic Management Systems:**
   - A traffic light control system with **99.99% availability** will have downtime limited to **52.60 minutes annually**, which is acceptable for maintenance intervals.


### **Importance of SLA and Availability Numbers**

1. **For Customers:**
   - SLA provides a benchmark for service reliability and sets the expectation for service uptime. Customers may claim compensation if the provider fails to meet SLA commitments.

2. **For Service Providers:**
   - SLA serves as a balance between operational costs and service reliability. Ensuring high availability often involves significant investments in infrastructure and process optimization.


### **Conclusion**

High availability is crucial for modern digital systems, especially those critical to business and public safety. Achieving **five nines (99.999%)** requires robust infrastructure, meticulous maintenance, and continuous monitoring, ensuring minimal downtime and maximal user trust.


---

## **Số liệu về khả năng sẵn sàng**

### **Khả năng sẵn sàng cao (High Availability - HA)**

**Khả năng sẵn sàng cao (High Availability)** đề cập đến khả năng của một hệ thống duy trì hoạt động liên tục trong một khoảng thời gian dài mà không gặp sự cố ngừng hoạt động. Khả năng sẵn sàng cao thường được biểu diễn dưới dạng phần trăm, với **100%** nghĩa là không có thời gian ngừng hoạt động. Trong thực tế, hầu hết các dịch vụ đạt mức khả năng sẵn sàng từ **99% đến 100%**.


### **Thỏa thuận mức độ dịch vụ (Service Level Agreement - SLA)**

**Thỏa thuận mức độ dịch vụ (SLA)** là hợp đồng chính thức giữa nhà cung cấp dịch vụ và khách hàng, định nghĩa mức độ **uptime** (thời gian hệ thống sẵn sàng) mà dịch vụ phải đảm bảo.

- Các nhà cung cấp dịch vụ đám mây hàng đầu như **Amazon**, **Google**, và **Microsoft** thường đặt SLA của họ ở mức **99.9% hoặc cao hơn**.
- Thời gian sẵn sàng (uptime) thường được biểu diễn bằng số "nines". Số lượng số 9 càng nhiều thì mức độ sẵn sàng càng cao và thời gian ngừng hoạt động càng ít.


### **Bảng so sánh thời gian ngừng hoạt động với mức khả năng sẵn sàng**

| **Khả năng sẵn sàng %** | **Thời gian ngừng hoạt động mỗi ngày** | **Thời gian ngừng hoạt động mỗi năm** |
|--------------------------|----------------------------------------|----------------------------------------|
| **99%**                 | 14.40 phút                            | 3.65 ngày                              |
| **99.9%**               | 1.44 phút                             | 8.77 giờ                               |
| **99.99%**              | 8.64 giây                             | 52.60 phút                             |
| **99.999%**             | 864.00 mili giây                      | 5.26 phút                              |
| **99.9999%**            | 86.40 mili giây                       | 31.56 giây                             |


### **Phân tích và ví dụ thực tế**

1. **Thời gian ngừng hoạt động giảm theo mức khả năng sẵn sàng cao hơn:**
   - Với **99% khả năng sẵn sàng**, hệ thống có thể gặp sự cố trong **14.40 phút mỗi ngày**, tương đương với **3.65 ngày mỗi năm**.
   - Với **99.999% khả năng sẵn sàng** ("năm số 9"), thời gian ngừng hoạt động chỉ còn **864 mili giây mỗi ngày**, tương đương khoảng **5.26 phút mỗi năm**.

2. **Ứng dụng thực tế của các mức khả năng sẵn sàng:**
   - **99%:** Phù hợp với các hệ thống không yêu cầu hoạt động liên tục, như các trang web cá nhân hoặc công cụ nội bộ.
   - **99.9%:** Thích hợp cho các ứng dụng thương mại điện tử, nơi thời gian ngừng hoạt động có thể ảnh hưởng nhẹ đến doanh thu.
   - **99.99% và cao hơn:** Được yêu cầu đối với các hệ thống quan trọng như chăm sóc sức khỏe, tài chính, và nền tảng đám mây lớn, nơi thời gian ngừng hoạt động có thể gây hậu quả nghiêm trọng.


### **Ví dụ thực tế**

1. **Trang web thương mại điện tử:**
   - Một trang web bán hàng với **99.9% khả năng sẵn sàng** có thể gặp thời gian ngừng hoạt động **1.44 phút mỗi ngày**. Trong khoảng thời gian này, khách hàng không thể đặt hàng.

2. **Ngân hàng trực tuyến:**
   - Một ngân hàng đạt **99.999% khả năng sẵn sàng** đảm bảo thời gian ngừng hoạt động tối đa chỉ **5.26 phút mỗi năm**, giúp duy trì các giao dịch liên tục cho khách hàng.

3. **Hệ thống quản lý giao thông IoT:**
   - Một hệ thống điều khiển đèn giao thông đạt **99.99% khả năng sẵn sàng** sẽ chỉ bị ngừng hoạt động tối đa **52.60 phút mỗi năm**, phù hợp với các kỳ bảo trì định kỳ.


### **Tầm quan trọng của SLA và số liệu về khả năng sẵn sàng**

1. **Đối với khách hàng:**
   - SLA cung cấp cơ sở để đánh giá độ tin cậy của dịch vụ và thiết lập kỳ vọng về thời gian hệ thống sẵn sàng. Khách hàng có thể yêu cầu bồi thường nếu nhà cung cấp không đáp ứng SLA đã cam kết.

2. **Đối với nhà cung cấp dịch vụ:**
   - SLA giúp cân bằng giữa chi phí vận hành và mức độ tin cậy của dịch vụ. Đảm bảo khả năng sẵn sàng cao thường yêu cầu đầu tư lớn vào cơ sở hạ tầng và tối ưu hóa quy trình.


### **Kết luận**

Khả năng sẵn sàng cao là yêu cầu cơ bản đối với các hệ thống kỹ thuật số hiện đại, đặc biệt là các hệ thống quan trọng đối với kinh doanh và an toàn công cộng. Đạt được **năm số 9 (99.999%)** không chỉ đòi hỏi cơ sở hạ tầng mạnh mẽ mà còn cần quy trình bảo trì chặt chẽ và giám sát liên tục, đảm bảo thời gian ngừng hoạt động tối thiểu và độ tin cậy tối đa.
