# Du_doan_gia_co_phieu
## Đoạn code trên bao gồm các bước để thực hiện một số công việc liên quan đến dữ liệu cổ phiếu và dự đoán giá cổ phiếu bằng mô hình hồi quy tuyến tính. Dưới đây là mô tả cho từng bước trong code:
- Import các thư viện cần thiết: Đầu tiên, các thư viện pandas, numpy, matplotlib.pyplot và seaborn được import để sử dụng trong quá trình xử lý dữ liệu và trực quan hóa.
- Đọc dữ liệu từ file CSV: Dữ liệu từ 4 file CSV được đọc vào DataFrame tương ứng với mỗi cổ phiếu (FPT, MSN, PNJ, VIC).
- Kết hợp các DataFrame: Các DataFrame đã đọc được kết hợp theo chiều dọc để tạo ra một DataFrame chứa dữ liệu của tất cả các cổ phiếu.
- Đổi tên các cột: Tên các cột của DataFrame được đổi lại để phù hợp với định dạng mong muốn.
- Chuyển đổi cột Date/Time về dạng chuẩn: Cột Date/Time được chuyển đổi sang định dạng datetime để có thể sử dụng trong việc trực quan hóa và tính toán thời gian.
- EDA (Exploratory Data Analysis): Quá trình khám phá dữ liệu bao gồm việc vẽ biểu đồ phân phối giá đóng cửa của từng cổ phiếu, biểu đồ tương quan giữa các biến, biểu đồ giá mở cửa và biểu đồ giá đóng cửa theo thời gian.
- Áp dụng mô hình dự đoán: Mô hình hồi quy tuyến tính được sử dụng để dự đoán giá cổ phiếu cho các ngày trong tương lai.
- Đầu tiên, mô hình được áp dụng cho cổ phiếu FPT. Dữ liệu cho cổ phiếu FPT được lọc và chuẩn bị để huấn luyện mô hình.
- Sau đó, dữ liệu được chia thành tập huấn luyện và tập kiểm tra.
- Mô hình hồi quy tuyến tính được huấn luyện trên tập huấn luyện.
- Dự đoán giá cổ phiếu cho tập kiểm tra được thực hiện và tính toán sai số bình phương trung bình gốc (RMSE).
- Tiếp theo, mô hình được sử dụng để dự đoán giá cổ phiếu cho các ngày trong tương lai trong khoảng thời gian 5 tháng.
- Dữ liệu dự đoán được trực quan hóa bằng cách vẽ biểu đồ
- Trực quan hóa kết quả dự đoán: Dữ liệu dự đoán cho cổ phiếu FPT được trực quan hóa bằng cách vẽ biểu đồ. Biểu đồ bao gồm các đường biểu diễn giá đóng cửa thực tế và giá đóng cửa dự đoán trong tương lai. Các đường này được vẽ trên cùng một trục thời gian để so sánh và đánh giá hiệu quả của mô hình.
- Lặp lại các bước 7 và 8 cho các cổ phiếu khác: Sau khi hoàn thành việc áp dụng mô hình cho cổ phiếu FPT, quá trình tương tự được lặp lại cho các cổ phiếu MSN, PNJ và VIC. Điều này giúp tạo ra dự đoán giá cổ phiếu và trực quan hóa kết quả cho tất cả các cổ phiếu.
## Cuối cùng, đoạn code trên cung cấp một quy trình hoàn chỉnh để thực hiện việc xử lý dữ liệu, huấn luyện mô hình hồi quy tuyến tính và dự đoán giá cổ phiếu trong tương lai. Nó giúp người dùng hiểu về cách dữ liệu được chuẩn bị, mô hình được huấn luyện và kết quả được trực quan hóa để phân tích và đưa ra quyết định đầu tư.
