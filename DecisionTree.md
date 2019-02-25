## Tại sao lại cần random_state trong khi khởi tạo Decision Tree trong scikitlearn?

The problem of learning an optimal decision tree is known to be NP-complete under several aspects of optimality 
and even for simple concepts. Consequently, practical decision-tree learning algorithms are based on heuristic algorithms 
such as the greedy algorithm where locally optimal decisions are made at each node. Such algorithms cannot guarantee to 
return the globally optimal decision tree. This can be mitigated by training multiple trees in an ensemble learner, 
where the features and samples are randomly sampled with replacement.
--> có quá nhiều yếu tố (feature) cần phải tối ưu 
--> không thể đảm bảo có thể cho ra một cây được tối ưu dựa trên toàn bộ yếu tố (feature)
--> huấn luyện nhiều cây cùng một lúc, ở mỗi cây thì các feature và ví dụ sẽ được lấy ra một cách ngẫu nhiên 


So, basically, a sub-optimal greedy algorithm is repeated 
a number of times using random selections of features and samples (a similar technique used in random forests). 
The random_state parameter allows controlling these random choices.
--> lặp lại một số lần ngẫu nhiên thuật toán greedy để tìm ra cây quyết định


If int, random_state is the seed used by the random number generator; 
If RandomState instance, random_state is the random number generator; 
If None, the random number generator is the RandomState instance used by np.random.
--> nếu chỉ định một số bất kì cho random_state thì kết quả của cây sẽ không bị thay đổi 
