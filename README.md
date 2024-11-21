<div align="center">

# Project - Machine Learning

</div>

## *Đề tài: Sử dụng phương pháp KNN, RandomForest, MLP để phân loại ảnh chó hay mèo trong xây dựng mô hình Machine Learning*
## 1. Công nghệ sử dụng
- **Frameworks**: 
  - `torch`
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `sklearn`
  - `PIL`
  - `os`
  - `seaborn`
  - `joblib`
  - `cv2`

## 2. Thuật toán
#### a. KNN (K-Nearest Neighbors)
<div style="text-align: justify;">

<strong>K-Nearest Neighbors (KNN)</strong> là một thuật toán học máy (Machine Learning), thường được sử dụng để phân loại hoặc hồi quy. Trong bài toán phân loại, KNN xác định nhãn cho một điểm dữ liệu mới bằng cách tìm kiếm "K" điểm dữ liệu gần nhất trong tập huấn luyện. Sau đó, nó gán nhãn cho điểm dữ liệu mới dựa trên sự đồng thuận của các nhãn trong số K điểm gần nhất đó.

</div>

**VD:**
<p align="center">
  <img src="https://images.datacamp.com/image/upload/v1686762721/image2_a2876c62d1.png" alt="" style="width: 70%; height: auto;">
<p align="right">
  <em>K-Nearest Neighbors (KNN) Classification with R Tutorial | DataCamp</em>
  
#### b. RandomForest
<div style="text-align: justify;">

<strong>Random Forest</strong> là một thuật toán học máy mạnh mẽ, dựa trên việc xây dựng nhiều cây quyết định (Decision Trees) và kết hợp kết quả của chúng để tăng độ chính xác và giảm ít lỗi nhất. Nó giống như một "rừng" nhiều cây, cùng làm việc để đưa ra dự đoán tốt nhất. Giúp tăng tính tin cậy, ổn định và rất mạnh mẽ trong xử lý dữ liệu phức tạp.

</div>

**VD:**
<p align="center">
  <img src="https://miro.medium.com/v2/resize:fit:1400/0*Ga2SY3cwKnkCRCTZ.jpg" alt="" style="width: 70%; height: auto;">
<p align="right">
  <em>Everything about Random Forest. Random Forest is one of the most… | by Abhishek Jain | Medium</em>

#### c. MLP
<div style="text-align: justify;">

<strong>MLP (Multilayer Perceptron)</strong> là một mô hình học máy thuộc nhóm mạng nơ-ron nhân tạo, nổi bật với khả năng mô phỏng các quan hệ phi tuyến tính phức tạp. MLP thường được sử dụng trong phân loại, hồi quy và nhận dạng mẫu. Mô hình này hoạt động bằng cách truyền dữ liệu qua nhiều tầng nơ-ron, từ đầu vào đến đầu ra, và sử dụng các thuật toán tối ưu hóa để điều chỉnh trọng số.
</div>

**VD:**
<p align="center">
  <img src="https://aiml.com/wp-content/uploads/2022/06/Multilayer-perceptron-MLP.png" alt="" style="width: 70%; height: auto;">
<p align="right">
  <em>What is a Multilayer Perceptron (MLP) or a Feedforward Neural Network (FNN)? - AIML.com</em>
  
## 3.  Dữ liệu sử dụng
<div style="text-align: justify;">

Dữ liệu cho bài toán phân loại hình ảnh này được thu thập từ Kaggle, mang tên "Animal Faces". Tập dữ liệu chứa một bộ sưu tập các hình ảnh khuôn mặt của mèo và chó, với nhiều góc độ, tư thế và bối cảnh khác nhau. Tất cả các hình ảnh đã được tải về và lưu trữ trong môi trường local, tạo điều kiện thuận lợi cho việc xử lý và phân tích dữ liệu. Gồm có hai tập Train set và Test set.
</div>

**Input:** Tập dữ liệu bao gồm nhiều hình ảnh của “cat” và “dog”.</br>
**Output:** Phân loại chính xác từng hình ảnh, xác định xem ảnh thuộc về "cat" hay "dog".

**VD:**
<p align="center">
  <img src="https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F793761%2Fafb6d1aa3be4c82e17a0d0b802436e82%2Fafhq_dataset.jpg?generation=1590130743209322&alt=media" style="width: 70%; height: auto;">
<p align="right">
  <em>Animal Faces | Kaggle </em>
  
## 4. So sánh và đánh giá các thuật toán 
<div style="text-align: justify;">

Trong ba thuật toán học máy phổ biến, KNN (K-Nearest Neighbors), MLP và RandomForest, MLP nổi bật hơn cả. KNN, mặc dù đơn giản và dễ triển khai, gặp khó khăn với dữ liệu lớn và bị ảnh hưởng bởi "cú pháp chiều". Random Forest có khả năng chống overfitting tốt và xử lý hiệu quả dữ liệu có chiều cao, nhưng mô hình phức tạp và tiêu tốn nhiều bộ nhớ. Ngược lại, MLP có khả năng học mối quan hệ phi tuyến phức tạp và xử lý tốt với dữ liệu lớn, mặc dù yêu cầu tài nguyên tính toán cao và cần tinh chỉnh kỹ thuật. Vì vậy, MLP được xem là lựa chọn tối ưu cho các bài toán phân loại hình ảnh.

</div>


