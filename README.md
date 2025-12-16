
# Hệ thống hỗ trợ quyết định canh tác  
Ứng dụng Machine Learning trong đánh giá điều kiện môi trường nông nghiệp

## Tổng quan

Kho lưu trữ này chứa mã nguồn của một hệ thống hỗ trợ quyết định canh tác (Decision Support System – DSS) được xây dựng nhằm đánh giá mức độ phù hợp canh tác dựa trên các yếu tố môi trường chính gồm lượng mưa, nhiệt độ không khí và độ ẩm.

Hệ thống áp dụng các kỹ thuật Machine Learning để phân loại mức độ canh tác và kết hợp với các quy tắc sinh thái – nông học nhằm sinh ra các khuyến nghị kỹ thuật có ý nghĩa thực tiễn. Mục tiêu của hệ thống là hỗ trợ người sử dụng trong quá trình ra quyết định, thay vì chỉ cung cấp kết quả dự đoán.

Ứng dụng được phát triển bằng Streamlit, phù hợp cho trình diễn nghiên cứu, thử nghiệm mô hình và triển khai trong các hệ thống nông nghiệp thông minh.

## Chức năng

- Nhập dữ liệu môi trường (lượng mưa, nhiệt độ, độ ẩm)
- Phân loại mức độ phù hợp canh tác theo ba mức: Thấp, Trung bình, Cao
- Sinh khuyến nghị canh tác theo các khía cạnh:
  - Chiến lược sản xuất
  - Quản lý nước
  - Điều tiết nhiệt độ và vi khí hậu
  - Nguy cơ sâu bệnh và sức khỏe hệ sinh thái
  - Quản lý đất và định hướng sản xuất bền vững

## Cấu trúc thư mục

Hệ thống hỗ trợ quyết định canh tác/

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

## Yêu cầu hệ thống

- Python 3.9 trở lên
- pip hoặc conda
- Windows, Linux hoặc macOS

## Cài đặt (Hướng dẫn cài đặt trên Vscode)

### Tải mã nguồn

Tải file Hệ thống hỗ trợ quyết định canh tác.zip, và mở file app.py

### Tạo môi trường ảo

python -m venv venv

Kích hoạt môi trường:

Windows:
venv\Scripts\activate

Linux / macOS:
source venv/bin/activate

### Cài đặt thư viện

pip install -r requirements.txt

## Vận hành ứng dụng

streamlit run app.py

Ứng dụng sẽ chạy tại địa chỉ:
http://localhost:8501

## Hướng dẫn sử dụng

1. Nhập các thông số môi trường.
2. Thực hiện phân tích trên giao diện.
3. Xem kết quả đánh giá mức độ canh tác.
4. Tham khảo các khuyến nghị kỹ thuật để hỗ trợ quyết định sản xuất.

## Mô hình Machine Learning

- Mô hình được huấn luyện trên dữ liệu môi trường lịch sử.
- Dữ liệu đầu vào được chuẩn hóa trước khi dự đoán.
- Kết quả mang tính hỗ trợ quyết định, không thay thế hoàn toàn chuyên gia.

## Giới hạn

- Chưa xét đến đặc thù từng loại cây trồng và điều kiện đất.
- Cần kết hợp với điều kiện địa phương và kinh nghiệm sản xuất.

## Định hướng phát triển

- Cá nhân hóa theo cây trồng và vùng sinh thái
- Tích hợp dữ liệu IoT và cảm biến
- Ứng dụng GIS và phân vùng canh tác
- Phân tích rủi ro và biến đổi khí hậu

## Tác giả

Tên tác giả: Phan Sơn Thịnh, Phạm Văn Hoàng Thiên, Phạm Sỹ Đức 
Lĩnh vực: Nông nghiệp thông minh, Machine Learning, Hệ thống hỗ trợ quyết định


