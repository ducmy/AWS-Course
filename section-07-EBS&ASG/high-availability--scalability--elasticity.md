### Scalability & High availability

**1. Scalability** có nghĩa là một app có thể handle những loader bởi sự đáp ứng.

Có 2 loại scalability:
- Vertical Scalability (Bề dọc, cố thể nói về chất lượng)
- Horizontal Scalability (Bề ngang, có thể nói về số lượng), hay còn được gọi là Elasticity

Scalability là khả năng mở rộng được liên kết, nhưng nó khác với High Availability

|Vertical Scalability |Horizontal Scalability|
|---|---|
|- Tăng size của instance <br>- Tăng kích cỡ EC2 t2.micro>>t2.large<br>- Thường dùng cho việc phân phối thệ thống như database<br>- Thường bị giới hạn bởi hardware|- Tăng số lượng intances, hoặc hệ thống cho app của bạn<br>- Ảnh hưởng gián tiếp đến phân phối hệ thống<br>- Thường sử dụng cho web/app hiện đại (microservices)|

**2. High availability**
- High availability thường đi chung với Horizontal scaling.
- Chạy app của bạn tối thiểu 2 Availability Zones.
- Cho lợi thế ngăn ngừa trung tâm data bị mất.

### **Summary:**
**Vertical Scaling**: tăng instance size 
**Horizontal Scaling**: tăng số lượng instance
- Auto Scaling Group
- Load Balancer
- 
**High Availability**
- Chạy những intance giống như khắp các AZ (across multi AZ)

### Scalability Vs Elasticity (Agility)
- Scalability: khă năng tăng load lớn hơn bằng sử dụng sức mạnh phần cứng mạnh hơn (scale up) hoặc thêm node (scale out)
- Elasticity: hệ thống scale dựa vào load(auto scaling), nó giống như là pay-per-use, dựa theo nhu cầu, tối ưu hóa chi phí
- Agility: giảm thiểu thời gian để tài nguyên đc triển khai nhanh chống, như việc giảm từ 1 tuần xuống vài phút.