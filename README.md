#HỆ THỐNG HỖ TRỢ QUYẾT ĐỊNH CANH TÁC

Decision Support System for Crop Cultivation Based on Machine Learning

1. Giới thiệu

Dự án này phát triển một hệ thống hỗ trợ quyết định canh tác (Decision Support System – DSS) dựa trên các yếu tố môi trường chủ đạo gồm lượng mưa, nhiệt độ không khí và độ ẩm. Hệ thống sử dụng mô hình Machine Learning để đánh giá mức độ phù hợp canh tác và cung cấp các khuyến nghị kỹ thuật có cơ sở sinh thái.

Mục tiêu của dự án không chỉ dừng lại ở việc dự đoán, mà hướng tới việc hỗ trợ ra quyết định trong bối cảnh sản xuất thực tế, nơi điều kiện môi trường luôn biến động và người sử dụng cần các gợi ý rõ ràng, có thể hành động được.

Ứng dụng được xây dựng bằng Streamlit nhằm phục vụ:

Trình diễn kết quả nghiên cứu

Thử nghiệm và đánh giá mô hình

Ứng dụng trong các hệ thống nông nghiệp thông minh

2. Chức năng chính

Hệ thống cung cấp các chức năng sau:

Nhập dữ liệu môi trường (thủ công hoặc từ nguồn bên ngoài)

Dự đoán mức độ phù hợp canh tác theo ba mức: Thấp, Trung bình, Cao

Sinh khuyến nghị canh tác theo nhiều khía cạnh:

Chiến lược sản xuất

Quản lý nước

Quản lý nhiệt độ và vi khí hậu

Rủi ro sâu bệnh và sức khỏe hệ sinh thái

Định hướng quản lý đất, dinh dưỡng và sản xuất dài hạn

Giao diện trực quan, dễ sử dụng, phù hợp cho cả người dùng kỹ thuật và người sản xuất

3. Cấu trúc thư mục
project/
│── app.py
│── README.md
│── requirements.txt
│
├── models/
│   ├── canh_tac_classifier.pkl
│   └── scaler.pkl
│
└── assets/
    └── background.png


Trong đó:

app.py: ứng dụng Streamlit chính

models/: chứa mô hình Machine Learning và bộ chuẩn hóa dữ liệu

assets/: tài nguyên giao diện

requirements.txt: danh sách các thư viện cần thiết

4. Yêu cầu hệ thống

Python phiên bản 3.9 trở lên

Trình quản lý gói pip hoặc conda

Hệ điều hành: Windows, Linux hoặc macOS

5. Cài đặt
5.1. Tải mã nguồn
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

5.2. Tạo môi trường ảo (khuyến nghị)
python -m venv venv


Kích hoạt môi trường:

Trên Windows:

venv\Scripts\activate


Trên Linux hoặc macOS:

source venv/bin/activate

5.3. Cài đặt các thư viện phụ thuộc
pip install -r requirements.txt

6. Vận hành hệ thống

Chạy ứng dụng Streamlit bằng lệnh:

streamlit run app.py


Sau khi khởi động thành công, ứng dụng sẽ được truy cập thông qua trình duyệt tại địa chỉ:

http://localhost:8501

7. Hướng dẫn sử dụng

Nhập các thông số môi trường gồm lượng mưa, nhiệt độ và độ ẩm.

Thực hiện phân tích bằng nút chức năng trên giao diện.

Quan sát kết quả đánh giá mức độ canh tác.

Tham khảo các khuyến nghị kỹ thuật được sinh ra để hỗ trợ ra quyết định.

8. Ghi chú về mô hình Machine Learning

Mô hình được huấn luyện trên tập dữ liệu khí hậu lịch sử.

Dữ liệu đầu vào được chuẩn hóa trước khi dự đoán.

Kết quả của mô hình mang tính hỗ trợ quyết định và không thay thế hoàn toàn vai trò của chuyên gia hoặc cán bộ kỹ thuật.

9. Giới hạn và lưu ý

Các khuyến nghị được xây dựng dựa trên các biến môi trường tổng quát, chưa xét đến đặc thù từng giống cây hoặc loại đất cụ thể.

Khi áp dụng trong thực tế, cần kết hợp với:

Điều kiện địa phương

Kinh nghiệm sản xuất

Thông tin dự báo thời tiết và thị trường

10. Hướng phát triển

Các hướng mở rộng tiềm năng của dự án bao gồm:

Cá nhân hóa khuyến nghị theo từng loại cây trồng

Tích hợp dữ liệu từ cảm biến và hệ thống IoT

Kết hợp bản đồ GIS để phân vùng sinh thái

Phân tích kịch bản biến đổi khí hậu

Đánh giá rủi ro và mức độ không chắc chắn của dự đoán

11. Tác giả

Tên tác giả: Phan Sơn Thịnh, Phạm Văn Hoàng Thiên, Phạm Sỹ Đức.
Lĩnh vực: Nông nghiệp thông minh, Machine Learning, Hệ hỗ trợ quyết định
