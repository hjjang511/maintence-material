1.	Bộ dữ liệu maintance

Bộ dữ liệu AI4I (AI for Industry 4.0) là một tập dữ liệu được xây dựng với mục tiêu hỗ trợ việc nghiên cứu và phát triển các giải pháp trí tuệ nhân tạo (AI) trong lĩnh vực công nghiệp, đặc biệt là công nghiệp sản xuất thông minh. Bộ dữ liệu này chứa các thông tin liên quan đến các quá trình sản xuất và hoạt động của máy móc trong môi trường sản xuất công nghiệp, bao gồm các chỉ số về trạng thái hoạt động, hiệu suất, và các yếu tố gây lỗi của thiết bị.

Bộ dữ liệu AI4I có các cột thông tin như sau:
•	UDI (Unique Device Identifier): Mã định danh duy nhất của thiết bị, giúp nhận diện từng mẫu dữ liệu một cách riêng biệt
•	Product ID: Mã sản phẩm được sản xuất, có thể liên quan đến loại sản phẩm hoặc lô sản phẩm cụ thể.
•	Type: Loại sản phẩm hoặc danh mục của sản phẩm, phân biệt các dòng sản phẩm khác nhau trong quá trình sản xuất.
•	Air Temperature [K]: Nhiệt độ không khí xung quanh máy móc trong quá trình sản xuất, tính bằng độ Kelvin (K).
•	Process Temperature [K]: Nhiệt độ tại điểm hoạt động của quá trình sản xuất, tính bằng độ Kelvin (K). Thường cao hơn nhiệt độ không khí do phát sinh nhiệt từ hoạt động máy móc.
•	Rotational Speed [rpm]: Tốc độ quay của động cơ, tính bằng vòng/phút (rpm), thể hiện tốc độ hoạt động của máy móc.
•	Torque [Nm]: Mô-men xoắn (torque), tính bằng Newton-mét (Nm), thể hiện lực quay của máy móc trong quá trình vận hành.
•	Tool Wear [min]: Độ mòn của dụng cụ sản xuất, tính bằng phút (min), biểu thị thời gian công cụ đã được sử dụng trong sản xuất. Đây là thông số quan trọng để đánh giá tình trạng của công cụ và                     khả năng cần bảo trì hoặc thay thế.
•	Target: Nhãn mục tiêu (target), xác định xem một sản phẩm có đạt tiêu chuẩn hay không. Đây có thể là biến nhị phân, cho biết sản phẩm đã qua kiểm tra chất lượng (đạt hoặc không đạt).
•	Failure Type: Loại lỗi gặp phải (nếu có) trong quá trình sản xuất. Các giá trị trong cột này có thể bao gồm:
   o	Không lỗi (No Failure)
   o	Lỗi quá tải công cụ (Tool Wear Failure)
   o	Lỗi nguồn nhiệt (Heat Dissipation Failure)
   o	Lỗi công cụ (Power Failure)
   o	Lỗi bôi trơn (Overstrain Failure)
   o	Lỗi môi trường (Random Failures)
Bộ dữ liệu này có thể được dùng để xây dựng các mô hình AI và phân tích dữ liệu, nhằm dự đoán lỗi hoặc tối ưu hóa hiệu suất của máy móc. Các cột Rotational Speed, Torque, và Tool Wear có thể đóng vai trò quan trọng trong việc phân tích sự hao mòn của máy móc và dự đoán thời điểm bảo trì cần thiết. Các cột Air Temperature và Process Temperature giúp đánh giá sự ảnh hưởng của nhiệt độ đến hiệu suất hoạt động và tuổi thọ của thiết bị.
2.	Bộ dữ liệu material
Bộ dữ liệu gồm 2 bảng: material.csv và Data.csv, gồm 15 đặc trưng mô tả các đặc điểm kĩ thuật của vật liệu và 1 nhãn. 
    Dưới đây là tổng quan về các đặc trưng:
•	Std: Tiêu chuẩn vật liệu hoặc mã định danh tiêu chuẩn (Standard).
•	ID: Mã định danh duy nhất của vật liệu.
•	Material: Loại vật liệu.
•	Heat treatment: Phương pháp xử lý nhiệt của vật liệu.
•	Su: Độ bền kéo (Ultimate tensile strength).
•	Sy: Giới hạn chảy (Yield strength).
•	A5: Độ giãn dài đến khi đứt (percentage elongation).
•	Bhn: Độ cứng Brinell của vật liệu.
•	E: Mô đun đàn hồi (Elastic modulus).
•	G: Mô đun cắt (Shear modulus).
•	mu: Hệ số ma sát (Friction coefficient).
•	Ro: Khối lượng riêng (Density).
•	pH: Độ pH, có thể liên quan đến tính chất hóa học bề mặt hoặc môi trường thử nghiệm.
•	Desc: Mô tả vật liệu hoặc chi tiết về mẫu thử.
•	HV: Độ cứng Vickers.
•	Use: Vật liệu có được sử dụng hay không



