## 🚲 Cyclistic Bike-Share Analysis (07/2024 - 06/2025)

## 📌 Giới thiệu
Dự án phân tích dữ liệu dịch vụ **Cyclistic Bike-Share** tại Chicago trong giai đoạn **07/2024 - 06/2025**, nhằm so sánh hành vi giữa **Member** và **Casual** để đề xuất chiến lược tăng tỷ lệ thành viên.

📊 [Xem báo cáo trực tiếp (GitHub Pages)](https://binhphan-da.github.io/Cyclistic_BikeShare-_Analysis_06_2025/)  
💻 [Xem toàn bộ code & dữ liệu](https://github.com/BinhPhan-DA/Cyclistic_BikeShare-_Analysis_06_2025)

---

## 🎯 Mục tiêu phân tích
- So sánh hành vi giữa **member** và **casual**.
- Phân tích xu hướng sử dụng theo thời gian, loại xe, địa điểm.
- Đề xuất chiến dịch marketing nhằm chuyển đổi casual thành member.
---

## 📊 Quy trình thực hiện

### 1. Thu thập & Làm sạch dữ liệu
- Tải dữ liệu thô từ [Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html).
- Import 12 file CSV vào **SQL Server**.
- Gộp dữ liệu thành một bảng tổng hợp.
- Loại bỏ bản ghi sai lệch:
  - `ride_length <= 0` hoặc `ride_length > 1440 phút`.
  - Thiếu tọa độ hoặc tên trạm.
  - Trùng `ride_id`.
- Kết quả: loại bỏ ~1,6% dữ liệu (không ảnh hưởng đáng kể).

### 2. Phân tích dữ liệu
- So sánh số lượng chuyến đi giữa **member** và **casual**.
- Phân tích thời lượng trung bình mỗi chuyến.
- Phân tích xu hướng sử dụng theo ngày trong tuần.
- Xác định loại xe phổ biến theo nhóm khách hàng.
- Liệt kê **Top 10 trạm xuất phát** phổ biến nhất cho từng nhóm.

### 3. Trực quan hóa dữ liệu
- Sử dụng **Excel** và **R (ggplot2)** để vẽ biểu đồ.
- Tạo báo cáo tự động bằng **R Markdown**.

---

## 📈 Kết quả chính
- **Member** chiếm ~63,6% tổng số chuyến đi.
- **Casual** có thời lượng chuyến dài hơn (~20,3 phút so với 11,9 phút).
- **Casual** tăng sử dụng mạnh vào cuối tuần; **member** ổn định cả tuần.
- **Electric bike** là loại xe được sử dụng nhiều nhất tổng thể.
- **Casual** hay bắt đầu ở các trạm gần khu du lịch; **member** ở khu văn phòng.

---

## 💡 Đề xuất
1. Chạy chiến dịch **"Dùng thử Member cuối tuần"** cho casual.
2. Tối ưu phân bổ xe điện ở trạm du lịch vào cuối tuần.
3. Thử nghiệm quảng cáo & ưu đãi khác nhau (A/B testing).

---

## 📥 Dữ liệu
- **Dữ liệu thô (.zip, 12 tháng)**: [📂 Tải tại đây](https://drive.google.com/file/d/1GOnSlufo8eqpkd1Bzqmh7K2tNdqCSKwC/view?usp=drive_link)
- **Dữ liệu đã làm sạch (.zip)**: [📂 Tải tại đây](https://drive.google.com/file/d/1cwUgTphiQwf5mk4v7ja6h881p4gTZVzn/view?usp=drive_link)

⚠ *Do giới hạn 100MB của GitHub, dữ liệu được lưu trữ trên Google Drive.*

---

## 🛠 Công nghệ sử dụng
- **SQL Server** – Làm sạch & xử lý dữ liệu.
- **Excel** – Trực quan hóa nhanh.
- **R (ggplot2, kableExtra)** – Biểu đồ & báo cáo.
- **GitHub** – Lưu trữ & chia sẻ dự án.

---

## 📄 Báo cáo
Báo cáo chi tiết kèm biểu đồ được lưu tại:  
[`Cyclistic_analysis.Rmd`](Cyclistic_analysis.Rmd) – có thể knit ra HTML/PDF.

---

## 👤 Tác giả
- **Phan Bá Bình**  
📧 Email: [binhphanit2109@gmail.com]  
🔗 GitHub: [https://github.com/BinhPhan-DA](https://github.com/BinhPhan-DA)
🔗 LinkedIn: [linkedin.com/in/yourprofile](https://www.linkedin.com/in/b%C3%ACnh-phan-aa4600350/) 
