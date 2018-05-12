# Machine Learning

### 2.1. Gausian mixture models
**sklearn.mixtures** là một package cho phép người ta học Gaussian Mixture Medels(diagonal, spherical, tired,and full convariance matrices support), sample them, và estimate chúng từ data. Các cơ sở giúp xác định số lượng thành phần thích hợp được cung cấp.
A Gausian mixture medel là một mô hình xác suất giả định tất cả các điểm dữ liệu được tạo ra từ hổn hợp của một số hữ hạn của Gaussian distributions với tham số không xác định. Người ta có thể nghỉ về mixture models như generalizing k-means clustering để kết hợp thông tin về cấu trúc convariance của dữ liệu cũng như các centes của the latent Gausians.</br>
Scikit-learn thực hiện các class khác nhau để ước tính Gaussian mixture models, tương ứng với các chiến lược ước tính khác nhau, chi tiết bên dưới.
#### 2.1.1. Gausian Mixture
The **GaussianMixture** object thực hiện ** expectation-maximization**(EM) thuật toán cho phù hợp mixture-of-Gaussion models. Nó cũng có thể vẽ confidence ellipsoids cho multivariate models, và tính toán the Bayesian Infomation Criterion để truy cập số clusters in the data.
A **GaussianMixture.fit** method is provided that learns a Gaussian Mixture Model from train data. Cho test data, Nó có thể gán mỗi sample the Gaussian nó chủ yếu có thể thuộc về việc sử dụng **GaussianMixture.predict** method.</br>

The GaussianMixture đi kèm với tùy chọn khác nhau để hạn chế convariance của the difference classes estimated: spherical, diagonal, tied or full convariance.
##### 2.1.1.1. Pros and cons of class ***GaussianMixture***
###### 2.1.1.1.1. Pros
Speed: Nó là thuật toán nhanh cho learning mixture models.</br>
Agnostic: Vì thuật  toán này tối đa hóa khả năng, Nó sẽ không thiên vị ý nghĩa về 0, or thiên vị kích thước cụm để có cấu trúc cụ thể mà có thể hoặc có thể không áp dụng.</br>
###### 2.1.1.1.2. Cons
**Singularities:** Khi không có đủ điểm cho mỗi mixture, ước tính matrices convariance trở nên khác nhau, và thuật toán được biết để phân ra và tìm giải pháp với khả năng vô hạn trừ khi một người thường xuyên hóa các hiệp phương sai nhân tạo.</br>
**Number of components:** Thuật toán này sẽ luôn sử dụng tất cả thành phần có thể truy cập tới, cần held-out data or infomation theoretical criteria để quyết định số lượng thành phần cần sử dụng trong tin hiệu bên ngoài.
#### 2.1.1.2. Selecting the number of components in a classical Gaussian Mixture Model
The BIC criterion có thể sử dụng để chọn số thành phần trong Gaussian Mixture một cách hiểu quả. Về lý thuyết, nó chỉ phục hồi đúng số lượng thành phần trong asymptotic regime(i.e. Nếu có nhiều dữ liệu và giả sử dữ liệu đã được tạo ra i.i.d từ mixture of Gaussian distribution). Lưu yes rằng sử dụng **Variational Bayesian Gausian mixture** tránh các đặc điểm kỹ thuật của số lượng thành phần của Gaussian mixture model.</br>


