### Millions of Users and Beyond

**[English Below]**

Mở rộng một hệ thống để hỗ trợ **hàng triệu người dùng** là một quá trình lặp đi lặp lại và đòi hỏi sự tối ưu hóa không ngừng. Những gì đã học trong chương này nhìn chung là đã đủ ổn. Tuy nhiên, để áp dụng vào thực tế thì cần có những tinh chỉnh và cải tiến thêm. Ví dụ: có thể cần tối ưu hóa hệ thống và tách hệ thống thành những dịch vụ nhỏ hơn (**Microservice**).

Tất cả các kỹ thuật trong chương này cung cấp nền tảng vững chắc để giải quyết các thách thức mới trong việc mở rộng hệ thống.

#### **Tóm Tắt Các Bước Mở Rộng Hệ Thống Đến Hàng Triệu Người Dùng**

1. **Giữ cho tầng web là stateless**:
   - Di chuyển session data ra khỏi web server và lưu trữ ở persistent data store.

2. **Xây dựng hệ thống dự phòng (redundancy) ở mọi tầng**:
   - Đảm bảo rằng mỗi tầng đều có cơ chế dự phòng để xử lý lỗi, tăng tính sẵn sàng của hệ thống.

3. **Cache dữ liệu tối đa**:
   - Sử dụng cache để giảm tải cho database và cải thiện hiệu suất.

4. **Hỗ trợ nhiều data center**:
   - Sử dụng các data center ở nhiều khu vực địa lý để giảm độ trễ và cải thiện trải nghiệm người dùng.

5. **Lưu trữ nội dung tĩnh trong CDN**:
   - Sử dụng CDN để phục vụ các nội dung tĩnh như hình ảnh, CSS, JavaScript, giúp giảm tải cho web server.

6. **Mở rộng tầng dữ liệu bằng sharding**:
   - Phân chia dữ liệu thành nhiều shard để cân bằng tải và quản lý dữ liệu hiệu quả hơn.

7. **Tách các tầng thành các dịch vụ độc lập**:
   - Decouple các thành phần của hệ thống để dễ dàng mở rộng và bảo trì.

8. **Giám sát và sử dụng công cụ tự động hóa**:
   - Sử dụng các công cụ giám sát để hiểu rõ trạng thái hệ thống và phát hiện sự cố sớm.
   - Tự động hóa các quy trình build, test, và deploy để cải thiện năng suất.

#### **Tổng hợp**

Nội dung của chương này tuy cơ bản nhưng rất quan trọng cho việc hiểu và thiết kế các hệ thống lớn -> give yourself a pat on the back, and come to next chapter.

---

Scaling a system to support **millions of users** is an **iterative process** that requires continuous optimization and refinement. The techniques learned in this chapter will take you a long way, but scaling beyond millions of users requires additional fine-tuning and new strategies. For example, you may need to optimize your system further and decouple it into smaller, more manageable services.

The techniques outlined in this chapter provide a solid foundation for tackling new challenges in scaling systems.

#### **Summary: Scaling a System to Millions of Users**

1. **Keep the web tier stateless**:
   - Move session data out of web servers and store it in a persistent data store.

2. **Build redundancy at every tier**:
   - Ensure each tier has redundancy mechanisms to handle failures and increase availability.

3. **Cache data as much as possible**:
   - Use caching to reduce database load and improve system performance.

4. **Support multiple data centers**:
   - Deploy data centers in different geographical locations to reduce latency and enhance user experience.

5. **Host static assets in CDN**:
   - Use a Content Delivery Network (CDN) to serve static content like images, CSS, and JavaScript, reducing the load on web servers.

6. **Scale the data tier with sharding**:
   - Partition data into shards to balance load and manage data effectively.

7. **Split tiers into individual services**:
   - Decouple system components into independent services for easier scaling and maintenance.

8. **Monitor and automate**:
   - Use monitoring tools to understand system health and detect issues early.
   - Automate build, test, and deployment processes to improve productivity.

#### **Sum Up**

Congratulations on reaching this milestone! You’ve made significant progress in understanding and designing scalable systems. Give yourself a pat on the back – you’ve done an excellent job!
