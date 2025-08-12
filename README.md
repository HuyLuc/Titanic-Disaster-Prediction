# Dự Án Dự Đoán Tỷ Lệ Sống Sót Thảm Họa Titanic

## Mô tả dự án
Dự án này sử dụng dữ liệu hành khách tàu Titanic để phân tích và dự đoán khả năng sống sót của hành khách dựa trên các thông tin cá nhân như giới tính, tuổi, hạng vé, số người đi cùng gia đình, v.v. Đây là một bài toán phân loại nhị phân trong học máy.

## Mục tiêu
- Khám phá và phân tích dữ liệu hành khách Titanic
- Trực quan hóa các yếu tố ảnh hưởng đến khả năng sống sót
- Chuẩn bị và làm sạch dữ liệu cho mô hình học máy
- Xây dựng mô hình dự đoán khả năng sống sót

## Cấu trúc thư mục
```
├── Data/
│   ├── Data_Titanic.csv         # Dữ liệu gốc
│   ├── Data_Titanic_OK.csv      # Dữ liệu đã xử lý (CSV)
│   └── Data_Titanic_OK.xlsx     # Dữ liệu đã xử lý (Excel)
├── Pic/
│   ├── data.png                 # Hình minh họa dữ liệu gốc
│   └── dataxl.png              # Hình minh họa dữ liệu đã xử lý
├── Titanic_disaster_prediction.ipynb  # Notebook chính
└── README.md                    # File mô tả dự án
```

## Dữ liệu
### Dataset Titanic (1309 hành khách)
Bộ dữ liệu chứa thông tin của 1309 hành khách với 12 thuộc tính:

| Thuộc tính | Mô tả |
|------------|--------|
| **PassengerId** | ID của hành khách |
| **Survived** | Biến mục tiêu (0: Không sống sót, 1: Sống sót) |
| **Pclass** | Hạng vé (1: Hạng nhất, 2: Hạng hai, 3: Hạng ba) |
| **Name** | Tên hành khách |
| **Sex** | Giới tính (Male/Female) |
| **Age** | Tuổi (năm) |
| **SibSp** | Số anh chị em/vợ chồng trên tàu |
| **Parch** | Số cha mẹ/con cái trên tàu |
| **Ticket** | Số hiệu vé |
| **Fare** | Giá vé |
| **Cabin** | Số cabin |
| **Embarked** | Cảng lên tàu (C: Cherbourg, Q: Queenstown, S: Southampton) |

## Nội dung notebook

### 1. Chuẩn bị dữ liệu
- Import các thư viện cần thiết (pandas, numpy, matplotlib, seaborn)
- Đọc và hiển thị thông tin tổng quan về dataset
- Kiểm tra cấu trúc dữ liệu

### 2. Khám phá dữ liệu (EDA - Exploratory Data Analysis)
- Phân tích thống kê mô tả
- Kiểm tra giá trị thiếu (missing values)
- Trực quan hóa phân phối các thuộc tính
- Phân tích mối quan hệ giữa các biến và tỷ lệ sống sót

### 3. Tiền xử lý dữ liệu
- Xử lý giá trị thiếu
- Chuyển đổi kiểu dữ liệu
- Mã hóa biến phân loại
- Tạo biến mới (feature engineering)

### 4. Kết quả
- Xuất dữ liệu đã xử lý ra file CSV và Excel
- Lưu trữ trong thư mục `Data/`

## Công nghệ sử dụng
- **Python 3.8+**
- **Thư viện:**
  - `pandas`: Xử lý và phân tích dữ liệu
  - `numpy`: Tính toán số học
  - `matplotlib`: Vẽ biểu đồ cơ bản
  - `seaborn`: Trực quan hóa dữ liệu nâng cao

## Cài đặt

### Yêu cầu hệ thống
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

## Hướng dẫn sử dụng

1. **Tải dự án về máy**
2. **Đảm bảo có file dữ liệu** `Data_Titanic.csv` trong thư mục `Data/`
3. **Mở Jupyter Notebook:**
   ```bash
   jupyter notebook
   ```
4. **Mở và chạy file:** `Titanic_disaster_prediction.ipynb`

## Kết quả đầu ra
Sau khi chạy notebook, bạn sẽ có:
- File `Data_Titanic_OK.csv`: Dữ liệu đã làm sạch định dạng CSV
- File `Data_Titanic_OK.xlsx`: Dữ liệu đã làm sạch định dạng Excel
- Các biểu đồ phân tích và trực quan hóa dữ liệu
- Hiểu biết sâu sắc về các yếu tố ảnh hưởng đến khả năng sống sót

## Insights chính
Từ phân tích dữ liệu, có thể rút ra một số kết luận:
- Giới tính ảnh hưởng mạnh đến khả năng sống sót
- Hạng vé cao (First Class) có tỷ lệ sống sót cao hơn
- Trẻ em có khả năng sống sót cao hơn người lớn
- Cảng lên tàu cũng có thể ảnh hưởng đến tỷ lệ sống sót

## Tác giả
**Thiều Huy Lực**
- Sinh viên Đại học Mỏ - Địa chất Hà Nội (HUMG)

## Liên hệ
- Tác giả: Thiều Huy Lực
- Trường: Đại học Mỏ - Địa chất Hà Nội (HUMG)
- Email: huyluc323@gmail.com

## Ghi chú
- Dự án được thực hiện với mục đích học tập và nghiên cứu
- Dữ liệu Titanic là bộ dữ liệu kinh điển trong khoa học dữ liệu
- Code được viết với nhiều comment để dễ hiểu và học tập

---
*Cập nhật: Tháng 8, 2025*
