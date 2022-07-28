# Fake-news-detection
1. Giới thiệu
 
  Khái niệm “phương tiện truyền thông” không phải một khái niệm quá đỗi xa lạ trong thế kỉ 21, nó xuất hiện đã lâu và ngày càng phát triển. Nó là một lĩnh vực rộng lớn và đa dạng bao gồm báo chí, các nền tảng xã hội (Facebook, Instagram, Twitter, …), blog, truyền hình, … Thông qua nó, chúng ta có thể tự do, chủ động tiếp cận và chia sẻ thông tin mới nhất một cách nhanh hơn bao giờ hết mà không phải tiêu pha một số tiền lớn. Đây là ưu điểm lớn nhất của những sản phẩm trong lĩnh vực phương tiện truyền thông nhưng cũng là nhược điểm để những kẻ mang ý xấu lợi dụng và truyền bá những thông tin giả (fake news).
  
  Thực tế, nhiều thông tin giật tít được đăng trên các trang báo trực tuyến, mạng xã hội cá nhân để câu lượt xem, lượt tương tác nhằm thu lợi quảng cáo hoặc nghiêm trọng là gây hại cho người khác. Việc kiểm soát fake news trở thành một vấn đề lớn và khó khăn trong thời buổi số hóa như hiện nay. Do đó, việc phát hiện fake news nhưng năm gần đây đã trở thành một lĩnh vực nghiên cứu mới và thu hút khá nhiều sự chú ý từ giới chuyên gia.
  
  Thực nghiệm này được thực hiện chỉ nhằm mục đích học tập và nghiên cứu.
 
2. Phương pháp sử dụng

  Tôi đã thực nghiệm bài toán trên môi trường Colab, bằng ngôn ngữ python.
  
  Lí thuyết vận dụng: LSTM, kĩ thuật nhúng từ (CBOW-Continuous Bag-of-Words) và một số thuật toán khác (Bernoulli  Naive Bayes, Multinomial  Naive Bayes và SVM)
  
  Độ đo sử dụng: độ chính xác, f1-score và ma trận nhầm lẫn.

3. Bộ dữ liệu

  Bộ dữ liệu được thu thập bởi phòng thí nghiệm nghiên cứu ISOT (Information Security and Object Technology) của đại học Victoria.
  
  Tập dữ liệu chứa hai loại bài báo: tin tức giả (fake news) và tin tức thật (real news). Bộ dữ liệu này được thu thập từ các nguồn trong thế giới thực. Real news được thu thập từ các bài báo trung từ trang web tin tức Reuters.com (Reuterѕ là một hãng cung cấp thông tin ᴠà tin tức toàn cầu). Đối với fake news, chúng được thu thập từ nhiều nguồn gồm các bài đăng trên Twitter, bài báo trên các trang web không đáng tin cậy đã bị Politifact (một tổ chức kiểm tra sự thật ở Hoa Kỳ) và Wikipedia gắn cờ. Tập dữ liệu chứa các loại bài báo khác nhau về các chủ đề khác nhau. Tuy nhiên, phần lớn nội dung các bài báo tập trung vào các chủ đề chính trị và tin tức thế giới.

4. Chú thích 

 Dữ liệu khá lớn nên tôi đã nén nó lại về dạng .zip.
 
 Về file code:
 
  - FakeReal.ipynb: CBOW + LSTM
  
  - FakeNews_NB_SVM.ipynb: CBOW + một số thuật toán khác

5. Tham khảo

  [1]Kaggle, "Fake and real news dataset," 2019. [Online]. Available: https://www.kaggle.com/clmentbisaillon/fake-and-real-news-dataset. [Accessed 9 2021].
  
  [2]A. Hadeer, T. Issa and S. Sherif , "Journal of Security and Privacy," Detecting opinion spams and fake news using text classification, pp. 127-128, 2018. 
  
  [3]Ahmed Hadeer, Issa Traore and Sherif Saad, Detection of Online Fake News Using N-Gram Analysis and Machine Learning Techniques, 2018. 
