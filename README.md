# Nhóm 5 - Image Classificaion Using CNN on Cifar-10

## Giới thiệu

- Dự án "Image Classification Using CNN" tập trung vào việc áp dụng mạng nơ-ron tích chập (CNN - Convolutional Neural Network) để giải quyết vấn đề phân loại hình ảnh. Mục tiêu chính là xây dựng một hệ thống có khả năng tự động học và nhận diện đối tượng trong hình ảnh với độ chính xác cao.

## Triển khai CNN bằng Python trên Google COLAB

- Run code Doancuoiky.iypnb bao gồm ( Cài đặt thư viện Keras , Import các thư viện cần thiết , Tải tập dữ liệu Cifar-10 , Chuẩn hóa dữ liệu , Xây dựng và huấn luyện đánh giá mô hình.)
- Ngoài ra sử dụng Thêm Data Aumentation , thêm lớp mô hình CNN , Learning Rate (Sheduler) , EarlyStopping , Optimizer(AdamW) để cài thiện độ chính xác.
- Thư mục ImageTestBenNgoai đã được chúng em tải từ trên mạng về để dự đoán
- Hoặc có thể tải bất kỳ hình ảnh nào từ trên mạng về để dự đoán
- Độ chính xác cao khi hình ảnh dễ nhận diện

## Tính năng tải hình ảnh từ bên ngoài để dự đoán

- Ctrl+Enter để chạy , giao diện hiện ra Choose File và Cancel Upload
- ![image](https://github.com/user-attachments/assets/87ca4e81-676f-4a6e-8728-497487b33d64)
- Tải lên hình ảnh: Nhấn nút **"Choose files"** để chọn một hình ảnh từ máy tính của bạn. Hình ảnh đã tải lên sẽ hiển thị trực tiếp trên giao diện Google Colab.
- ![image](https://github.com/user-attachments/assets/27b2d64e-4116-424c-925a-6695968ccf8d)
- Dự đoán hình ảnh với độ chính xác dự đoán
- ![image](https://github.com/user-attachments/assets/1ad13433-024a-4c78-9516-b11f102a4751)
- Tự động save images sau khi dự đoán
- ![image](https://github.com/user-attachments/assets/02dc4956-d7d3-4bd4-acf3-df904d5e6fbd)

## Phân tích kết quả

- Độ chính xác của tập huấn luyện(Train) sau 40 epochs này là 0.7697 (hay 76.97%).
- Mất mát (loss) của tập huấn luyện(Train) sau epoch này là 0.6855.
- Độ chính xác của tập kiểm tra(Test) sau 40 epochs này là 0.8110 (hay 81.10%).
- Mất mát (loss) của tập kiểm tra(Test) sau epoch này là 0.5818.
- Tốc độ học (learning rate) là 0.000125.

## Phân tích kết quả tính năng dự đoán hình ảnh từ bên ngoài :

- Tỷ lệ chính xác sẽ Rất cao khi hình ảnh đầu vào trực quan rõ vật , dễ nhận diện .
- Deer và Horse : sẽ có thể nó nhận định sai Horse là Deer, vì nếu hình ảnh đầu vào Horse (nếu con Horse gầy ốm ).
- Nếu hình ảnh con vật nếu ở vị trí cao trong ảnh, nó sẽ nhận diện là Bird.
- Còn dường như Automobile, Ship , Truck , Airplane tỷ lệ chính xác rất cao và tỷ lệ đoán sai rất ít(hoặc dường như không có).
- Tỷ lệ đoán sai : Phần lớn là do hình ảnh đầu vào , ngoài ra tỷ lệ chính xác Mô hình của tâp Train (76.97%), Test(81.10%) vẫn còn hạn chế.

## Lời Cảm Ơn

Cảm ơn thầy Nguyễn Thái Anh và Trường Đại học Văn Lang đã tạo điều kiện để Nhóm 5 chúng em thực hiện đồ án một cách suôn sẻ. Trong quá trình làm còn nhiều thiếu sót nhưng những lời góp ý và sự giúp đỡ của thầy, nhóm chúng em đã có thể hoàn thành đồ án một cách trọn vẹn.

**Thành viên Nhóm 5**
|STT|Tên thành viên|MSSV|Nhiệm vụ|
|---|--------------|----|--------|
|1|Nguyễn Hữu Trường| 207CT65867|Nhóm trưởng|
|2|Thái Quốc Bảo|207CT09955|Thành viên|
|3|Đào Duy Luân|2174802010599|Thành viên|
|4|Lê Gia Hào|207CT65580|Thành viên|
