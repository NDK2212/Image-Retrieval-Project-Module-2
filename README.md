
# Project Image Retrieval Module 2

## Giới thiệu

Dự án Image Retrieval là một hệ thống truy xuất ảnh từ một tập hợp dữ liệu ảnh dựa trên các đặc trưng nội dung của ảnh, như màu sắc, hình dạng, và texture. Hệ thống cho phép người dùng tải lên một ảnh truy vấn và tìm kiếm những ảnh tương đồng trong cơ sở dữ liệu dựa trên khoảng cách của các vector đặc trưng. Dự án này được phát triển với mục đích nghiên cứu và triển khai các kỹ thuật truy xuất ảnh hiệu quả trong lĩnh vực xử lý ảnh và học máy.

## Các thành phần chính

- **Trích xuất đặc trưng (Feature Extraction)**: Áp dụng các kỹ thuật xử lý ảnh để trích xuất các đặc trưng quan trọng của ảnh như màu sắc, hình dạng và texture.
- **So sánh đặc trưng (Feature Comparison)**: Tính toán khoảng cách giữa các vector đặc trưng để so sánh độ tương đồng giữa các ảnh.
- **Truy xuất ảnh (Image Retrieval)**: Tìm kiếm và trả về các ảnh có đặc trưng tương tự với ảnh truy vấn dựa trên khoảng cách tính toán.

## Cài đặt

### Yêu cầu hệ thống

- Python 3.x
- Các thư viện Python:
  - NumPy
  - OpenCV
  - Scikit-learn
  - Matplotlib
  - Flask (cho giao diện web)

### Hướng dẫn cài đặt

1. **Clone repository**:
   ```bash
   git clone https://github.com/username/image-retrieval.git
   cd image-retrieval
   ```

2. **Cài đặt các thư viện cần thiết**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Chạy ứng dụng**:
   ```bash
   python app.py
   ```

4. Truy cập ứng dụng tại `http://localhost:5000` trên trình duyệt của bạn.

## Cấu trúc thư mục

- `app.py`: Tập tin chính để chạy ứng dụng web.
- `static/`: Chứa các tài nguyên tĩnh như ảnh và CSS.
- `templates/`: Chứa các tập tin HTML cho giao diện người dùng.
- `features_extraction.py`: Mã nguồn dùng để trích xuất đặc trưng từ ảnh.
- `image_retrieval.py`: Mã nguồn để thực hiện tìm kiếm ảnh dựa trên đặc trưng.
- `data/`: Chứa cơ sở dữ liệu ảnh.

## Sử dụng

1. Mở ứng dụng web.
2. Tải lên một ảnh truy vấn từ máy tính của bạn.
3. Hệ thống sẽ phân tích ảnh và trả về danh sách các ảnh tương đồng từ cơ sở dữ liệu dựa trên các đặc trưng đã trích xuất.

