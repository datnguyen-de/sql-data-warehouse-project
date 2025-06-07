Mô hình thử nghiệm datawarehouse
Dự án này trình bày một giải pháp phân tích và kho dữ liệu toàn diện, từ việc xây dựng kho dữ liệu đến việc tạo ra các thông tin chi tiết hữu ích. Được thiết kế như một dự án cá nhân (portfolio), nó làm nổi bật các phương pháp hay nhất trong ngành về kỹ thuật và phân tích dữ liệu.

🏗️ Kiến trúc dữ liệu
Kiến trúc dữ liệu cho dự án này tuân theo Kiến trúc Medallion với các lớp Bronze, Silver, và Gold:

Lớp Bronze (Đồng): Lưu trữ dữ liệu thô nguyên trạng từ các hệ thống nguồn. Dữ liệu được nhập từ các tệp CSV vào Cơ sở dữ liệu SQL Server.
Lớp Silver (Bạc): Lớp này bao gồm các quy trình làm sạch, chuẩn hóa và bình thường hóa dữ liệu để chuẩn bị cho việc phân tích.
Lớp Gold (Vàng): Chứa dữ liệu sẵn sàng cho nghiệp vụ được mô hình hóa theo lược đồ hình sao (star schema) cần thiết cho việc báo cáo và phân tích.
