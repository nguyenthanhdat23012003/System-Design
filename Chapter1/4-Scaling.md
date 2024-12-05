
**[Vietnamese Below]**

## Vertical Scaling vs Horizontal Scaling

When scaling a system, there are two main approaches: **Vertical Scaling** (Scale Up) and **Horizontal Scaling** (Scale Out). Let’s dive deeper into these methods.

### Vertical Scaling (Scale Up)

Vertical scaling, also known as **scale up**, is the process of adding more resources (RAM, CPU, etc.) to an existing server. This is a suitable option for systems with low traffic due to its simplicity.

- **Advantages**:
  - Easy to implement by upgrading hardware (RAM, CPU, etc.) on the existing server.
  - Requires minimal changes to the system architecture.

- **Limitations**:
  - **Physical Limits**: A single server has limitations on how much CPU and RAM it can accommodate.
  - **No Redundancy**: If the single server fails, the entire system goes down.

Vertical scaling is ideal for small systems or applications with low traffic where the cost of upgrading hardware is lower than restructuring the system.

### Horizontal Scaling (Scale Out)

Horizontal scaling, also known as **scale out**, allows systems to scale by adding multiple servers to a resource pool. This approach is more common for large-scale applications due to its scalability.

- **Advantages**:
  - **High Scalability**: New servers can be added as needed to handle increased demand.
  - **Better Fault Tolerance**: If one server fails, other servers in the system can continue to operate.

- **Limitations**:
  - **Complexity**: Requires significant changes to the system architecture.
  - **Load Balancing Requirement**: Needs a load balancer to distribute traffic evenly across servers.

### Integrating Load Balancer with Horizontal Scaling

In the previous design, users were directly connected to the web server. If the server goes offline or becomes overloaded, users experience slow responses or failed connections. A load balancer is the best solution to address these issues.

- **Load Balancer**:
  - Distributes incoming traffic evenly across servers.
  - Minimizes the risk of server overload or failure.
  - Enhances system availability and performance.

### Conclusion

- **Vertical Scaling** is suitable for small systems or low-traffic applications due to its simplicity and lower cost.
- **Horizontal Scaling** is better for large systems requiring high performance and availability but involves higher complexity and cost to implement.

------------------

## Mở rộng theo chiều dọc và mở rộng theo chiều ngang

Khi mở rộng hệ thống, có hai phương pháp chính: **Vertical Scaling** (Scale Up) và **Horizontal Scaling** (Scale Out). Hãy cùng tìm hiểu kỹ hơn về hai phương pháp này.

### Vertical Scaling (Scale Up)

Vertical scaling, hay còn gọi là **scale up**, là quá trình cấp thêm tài nguyên (RAM, CPU, v.v.) cho máy chủ hiện tại. Đây là một lựa chọn phù hợp khi lưu lượng truy cập thấp nhờ tính đơn giản của nó.

- **Ưu điểm**:
  - Dễ dàng triển khai bằng cách nâng cấp phần cứng (RAM, CPU, v.v.) trên server hiện tại.
  - Không yêu cầu thay đổi lớn về kiến trúc hệ thống.

- **Hạn chế**:
  - **Giới hạn vật lý**: Một máy chủ có giới hạn về khả năng nâng cấp CPU và RAM, không thể mở rộng vô hạn.
  - **Không có khả năng chịu lỗi và dự phòng**: Nếu máy chủ duy nhất gặp sự cố, toàn bộ hệ thống sẽ ngừng hoạt động.

Vertical scaling thường phù hợp với các hệ thống có lưu lượng truy cập thấp hoặc các ứng dụng nhỏ, nơi chi phí nâng cấp phần cứng thấp hơn so với việc xây dựng lại kiến trúc hệ thống.

### Horizontal Scaling (Scale Out)

Horizontal scaling, hay còn gọi là **scale out**, cho phép mở rộng hệ thống bằng cách thêm nhiều máy chủ vào cụm tài nguyên (resource pool). Đây là phương pháp phổ biến hơn cho các ứng dụng quy mô lớn do khả năng mở rộng linh hoạt.

- **Ưu điểm**:
  - **Khả năng mở rộng cao**: Có thể thêm nhiều máy chủ để đáp ứng nhu cầu tăng cao.
  - **Chịu lỗi tốt hơn**: Nếu một máy chủ gặp sự cố, các máy chủ khác trong hệ thống vẫn có thể hoạt động bình thường.

- **Hạn chế**:
  - **Độ phức tạp cao**: Đòi hỏi thay đổi lớn về kiến trúc hệ thống.
  - **Yêu cầu cơ chế Load Balancing**: Cần sử dụng load balancer để phân phối công việc đều giữa các máy chủ.

### Kết Hợp Load Balancer với Horizontal Scaling

Trong thiết kế trước đây, người dùng kết nối trực tiếp với web server. Nếu web server bị offline hoặc quá tải, người dùng sẽ không thể truy cập hệ thống, dẫn đến phản hồi chậm hoặc mất kết nối. Load balancer là giải pháp tốt nhất để giải quyết các vấn đề này.

- **Load Balancer**:
  - Phân phối lưu lượng truy cập đều đến các máy chủ.
  - Giảm thiểu tình trạng một máy chủ bị quá tải hoặc gặp sự cố.
  - Tăng tính sẵn sàng (availability) và hiệu năng hệ thống.


### Kết Luận

- **Vertical Scaling** phù hợp với các hệ thống nhỏ hoặc các ứng dụng có lưu lượng truy cập thấp nhờ tính đơn giản và chi phí thấp.
- **Horizontal Scaling** là lựa chọn tốt hơn cho các hệ thống lớn, yêu cầu hiệu năng cao và tính sẵn sàng, nhưng đòi hỏi nhiều công sức và chi phí để triển khai.
