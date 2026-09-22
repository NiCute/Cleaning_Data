# 📊 Maven Toys: Sales & Profitability Analysis (End-to-End Project)

## 📌 Tổng quan dự án (Project Overview)
Đây là một dự án phân tích dữ liệu toàn diện (End-to-End Data Analytics) mô phỏng bài toán kinh doanh thực tế của chuỗi bán lẻ Maven Toys. Mục tiêu của dự án là bóc tách hiệu suất kinh doanh, định vị các nhóm sản phẩm sinh lời cao nhất và phân tích biến động doanh thu theo chuỗi thời gian nhằm đưa ra các quyết định tối ưu hóa vận hành.

## 🛠️ Luồng xử lý & Công nghệ (Tech Stack & Pipeline)
1. **Data Preparation (Python / Pandas):** 
   - Làm sạch bộ dữ liệu giao dịch thô (hơn 800,000 dòng).
   - Xử lý lỗi định dạng tiền tệ (chuyển chuỗi Text sang Float) và xử lý dữ liệu thiếu (Missing values).
   - Khai phá đặc trưng (Feature Engineering) để tính toán Doanh thu (Revenue) và Lợi nhuận (Profit).
2. **Exploratory Data Analysis (SQL / SQLite):** 
   - Triển khai In-memory Database ngay trong luồng Python để tối ưu tốc độ truy vấn.
   - Sử dụng SQL (`GROUP BY`, `ORDER BY`, `SUM`) để tổng hợp và phân lớp lợi nhuận theo danh mục.
3. **Data Visualization (Power BI):** 
   - Thiết kế Interactive Dashboard trực quan hóa KPI và xu hướng.
   - Áp dụng Cross-filtering giúp người dùng cuối (End-user) dễ dàng tương tác và tự khám phá dữ liệu.

## 💡 Thấu hiểu Kinh doanh (Key Business Insights)
Dựa trên báo cáo Dashboard, hệ thống ghi nhận các điểm nhấn sau:
* **Hiệu suất Tổng thể:** Tổng doanh thu toàn hệ thống đạt mức **$14.44 Triệu** trong giai đoạn phân tích.
* **"Con gà đẻ trứng vàng":** Danh mục **Toys (Đồ chơi)** là mũi nhọn kinh doanh khi mang về lợi nhuận cao nhất (vượt mốc $1.0M), bám sát phía sau là nhóm *Electronics*. Ở chiều ngược lại, *Sports & Outdoors* có biên lợi nhuận mỏng nhất.
* **Xu hướng bùng nổ:** Tốc độ tăng trưởng của năm 2023 vượt trội hoàn toàn so với 2022. Đỉnh điểm bùng nổ doanh thu lịch sử được ghi nhận vào **giai đoạn tháng 4 - tháng 5/2023**, chạm ngưỡng gần **$70,000/ngày**.

## 🚀 Đề xuất Chiến lược (Business Recommendations)
1. **Tối ưu Danh mục & Ngân sách:** Phân bổ 60-70% ngân sách Marketing và diện tích quầy kệ cho 2 nhóm hàng chủ lực là *Toys* và *Electronics* để tối đa hóa lợi nhuận. Đồng thời, cần đánh giá lại chi phí lưu kho của nhóm *Sports & Outdoors*.
2. **Quản trị Tồn kho theo Mùa vụ:** Dựa vào chu kỳ bùng nổ doanh thu, bộ phận Chuỗi cung ứng (Supply Chain) cần tăng cường trữ lượng hàng hóa nhập kho từ tháng 3 để sẵn sàng đáp ứng lượng cầu khổng lồ của đợt sóng tháng 4 - tháng 5, tránh nguy cơ đứt gãy hàng hóa (Out-of-stock).
3. **Chiến dịch Kích cầu:** Vào các khoảng thời gian "thung lũng" (doanh thu chạm đáy), cần triển khai các chiến dịch xả kho giảm giá hoặc bán chéo (Cross-selling) để giải phóng hàng tồn và duy trì dòng tiền ổn định.
