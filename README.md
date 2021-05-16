# Final Project in Introduction to Machine Learning Spring 2021
## SincNet Architecture and the paper Speaker Recognition from raw waveform with SincNet - Mirco Ravanelli, Yoshua Bengio

### Phần mở đầu

Trong những năm gần đây, Machine Learning (Học máy/ Máy học) đạt được rất nhiều thành tựu nổi bật, thúc đẩy Cách mạng Công nghệ 4.0 phát triển nhanh chóng. Một trong những tác nhân chính mạnh mẽ nhất đến từ Deep Learning (Deep Neural Networks - Các mạng Học sâu), các mô hình học dựa trên những phương pháp này đã rất thành công, đạt được một hiệu năng đầy triển vọng, trong nhiều tác vụ khác nhau như Thị giác Máy tính (Computer Vision), Nhận dạng Nhân trắc học (Biometrics): Giọng nói (Speech), Khuôn mặt (Face), Vân tay (Fingerprint), ..., Xử lý ngôn ngữ tự nhiên (Natural Language Processing), ...
	
Trong tác vụ nhận dạng, đặc biệt là nhận dạng giọng nói (Voice/ Speech Recognition) gần như là một bài toán khó trong nhiều năm, cần những phương pháp rất phức tạp để có thể giải quyết được. Nhờ vào Học sâu, phương giải phải khả thi, mà cụ thể là với Mạng Neural Tích chập (Convolutional Neural Networks - CNNs) đem lại những kết quả đầy hứa hẹn khi chỉ cần đầu vào trực tiếp là mẫu giọng nói thô. Thay vì sử dụng các tính năng thủ công tiêu chuẩn, CNNs sau này học cách biểu diễn giọng nói cấp thấp từ các dạng sóng, có khả năng cho phép mạng nắm bắt tốt hơn các đặc điểm giọng nói ở dải tần hẹp quan trọng như cao độ và hình dạng.
	
Với mục đích tìm hiểu bài báo khoa học, cũng như tìm hiểu những mô hình, phương pháp Học máy nổi bật gần đây trong những tác vụ quan trọng, mà cụ thể là nhận dạng. Nhóm chúng em quyết định chọn một bài báo khoa học làm tài liệu thực hiện chính cho đồ án môn học

### Giới thiệu

Như chúng ta đã biết rằng giọng nói (voice/speech) là một đặc điểm sinh trắc học (nhân trắc học) dễ dàng tiếp cận nhất mà không cần phải có thêm thiết bị thu nhận và hệ thống truyền dẫn bởi vì lý do của sự gia tăng mỗi ngày số người sử dụng điện thoại di động giao tiếp với nhau. Tuy nhiên, đặc điểm giọng nói không chỉ liên quan đến các đặc trưng cá thể mà còn liên quan với môi trường xung quanh và vấn đề xã hội. May mắn thay, các công nghệ và ứng dụng tiên tiến có thể khắc phụ những vấn đề trên, cho phép cải thiện độ hiệu quả và tin cậy cho việc xác nhận từ xa hoặc nhận diện giọng nói chỉ dựa vào tín hiệu giọng nói truyền qua sóng điện thoại. 

Hầu hết những giải pháp "state of the art" đều dựa trên việc biểu diễn {i-vectors của những đoạn giọng nói, cải thiện đáng kể so với mô hình Gaussian Mixture Model-Universal Background Models (GMM-UBMs).
	
Trong những năm gần đây, Trí tuệ Nhân tạo nhất là lĩnh vực Học máy (Machine Learning) đạt được nhiều thành tựu nổi bật là nhờ Học Sâu (Deep Learning). Các mạng học sâu - Deep Neural Networks (DNNs) sử dụng trong những framework i-vector để tính toán thống kê Baum-Welch hoặc trong các khung rút trích đặc trưng theo mức (frame-level feature extraction). Ngoài ra, DNNs còn được dùng trong việc phân tách/ phân loại giọng nói.
	
Những kỹ thuật này cần phải tuân theo một số tiêu chuẩn nhất định, ví dụ như: độ mượt của tần số giọng nói có thể làm cản trở việc rút trích một số đặc trưng của giọng nói như cao độ và ngữ âm, .... Để khắc phục chúng, các công trình mới đây thường dùng kỹ thuật spectrogram bins (bin tần số) hoặc dùng cả sóng thô (raw waveform).

### Những việc làm ở giữa kỳ

Các đóng góp Giữa kỳ:
- Tìm hiểu về lĩnh vực Nhận dạng giọng nói
- Tìm hiểu phương pháp, kiến trúc mạng nổi bật gần đây nhất: SincNet Architecture từ bài báo Speaker Recognition from raw waveform with SincNet, Mirco Ravanelli, Yoshua Bengio
- Trình bày kiến trúc mạng, chứng minh công thức theo hướng dẫn từ bài báo
- Quay video thuyết trình những gì tìm hiểu được. 

### Những việc làm ở cuối kỳ

(Dự kiến)
- Chuẩn bị dữ liệu (cho tiếng Anh và tiếng Việt).
- Xây dựng mô hình.
- Trực quan hóa, đánh giá mô hình.
- Nhận xét những kết quả làm được.

### Lời bình luận cuối

### Đóng góp

- Issue Tracker: github.com/nhutnamhcmus/introduction-to-machine-learning-hcmus-presentation/issues
- Source Code: github.com/github.com/nhutnamhcmus/introduction-to-machine-learning-hcmus-presentation

### Hỗ trợ/ Liên hệ

Email report: lenam.fithcmus@gmail.com/ namele1232000@gmail.com

### Giấy phép

MIT license

### Lời cảm ơn chân thành

Trong lời cuối cùng này, chúng em muốn cảm ơn các tác giả của bài báo về Speaker Recognition from raw waveform with SincNet, những người đã tạo ra một kiến trúc tuyệt vời - SincNet, một kiến trúc neural nhân tạo để xử lý hiệu quả các mẫu âm thanh thô và video YouTube của Giáo sư, hướng dẫn và giải thích rất chi tiết, phần nào giúp chúng em hoàn thành việc học tập này.

Chúng em cũng muốn gửi lời cảm ơn đến các thầy cô giáo, trợ giảng và người bạn cùng lớp đã giúp đỡ chúng em hoàn thành đồ án này và bài thuyết trình này.

------------------------------------------------------
### Abstract 

In recent years, Machine Learning has achieved many outstanding achievements, promoting the rapid development of Technology Revolution 4.0. One of the most powerful factors coming from Deep Learning, learning models based on these methods have been very successful, achieving a promising performance, for many various tasks in Computer Vision, Natural Language Processing, Pattern Recognition, Biometrics Recognition, ...

In recognition task, especially Voice/ Speech Recognition is almost a difficult problem for many years, it takes very complicated methods to solve. Due to Deep Learning, the solution must be feasible, especially with Convolutional Neural Networks (CNNs) that bring promising results when only direct input is the raw voice sample. Instead of using standard manual features, CNNs later learned to represent low-level voices from waveforms, potentially allowing the network to better capture critical narrow-band speaker characteristics such as pitch and formants.

For the purpose of researching scientific articles, as well as finding out machine learning models and methods that have emerged recently in important tasks, namely identification. Our group decided to choose a scientific paper as the main implementation document for the subject project.

### Acknowledgments

Our work would not be complete without the enthusiastic help from our teachers, our friends, our team. Thank you for our family always support us during the time. Last but not least, we must thank to the authors of the Handbook of Biometrics, who wrote a usefull science book for newbie in Machine Learning like us, the authors of papers that we reference for this project, the authors of SincNet - a great architecture.

### Introduction 

As we know about voice is the most accessible biometric trait as no extra acquisition device or transmission system is needed because more and more people all over the world use mobile phone to talk together, the number of telephone landlines in operation increase everyday and the development of social network. However, the voice trait is not only related with personal characteristics, but also with many environmental and sociolinguistic variables. Fortunately, state-of-the-art technologies and applications are presently able to compensate for all those sources of variability allowing for efficient and reliable value-added applications that enable remote authentication or voice detection based just in telephone-transmitted voice signals. Moset of these state of the art methods based on the i-vectors representation of speech segments, significantly improved over the Gaussian Mixture Model-Universal Background Models and development of the Deep Neural Network contributed to the resolution of perception. voice form. However, there are still many problems to be solved with this problem such as the input data problem, optimizing the error, increasing the convergence performance and especially how to design a compact, fine-tunable model. are to match our applications.

### About our working in midterm

Content outline for our work in in midterm following the list below:
- Introduction
- The motivation of Voice/ Speech Recognition
- Problem statement
- Approach methods
- About the paper - Speaker Recognition from raw waveform with SincNet
    - Introduction about this paper
        - Speaker Recognition
        - Convolution Neural Networks and its problem when processing speech signal
    - The SincNet Architecture
        - The idea from Digital Signal Processing
        - Custome CNNs filter
        - Go back to time domain by using Fourier Transformation
    - Experimental
        - Corpus/ Dataset
        - Build SincNet Architecture: How the authors build and config it
        - Compara SincNet to CNN
    - Some results
        - In speaker verification task
        - In speaker identification task

### About our working in endterm

We will use SincNet to train a model use in speaker verification task and speaker identification task, we use three dataset: TIMIT dataset, Librispeech Dataset (for English) and Son el Dataset for Vietnamese

To present a Speaker Recognition pipeline:

- Data prepration
- Development: Training model
- Enrollment: Enroll for new people
- Evaluate: Testing model, compute d-vector and use cosine meansure to identify or verify speaker

### Final comment

### Contribute

- Issue Tracker: github.com/nhutnamhcmus/introduction-to-machine-learning-hcmus-presentation/issues
- Source Code: github.com/github.com/nhutnamhcmus/introduction-to-machine-learning-hcmus-presentation

### Support

If you are having issues, please let us know. We have a mailing list located at: lenam.fithcmus@gmail.com or namele1232000@gmail.com

### License

The project is licensed under the MIT license.

### Acknowledgments

In this final words, we would like to thank the authors of the paper Speaker Recognition from raw waveform with SincNet, who created a great architecture - the SincNet, a neural architecture for efficiently processing raw audio samples and his YouTube video, which guide us to follow this paper.

We also would like to thank our teachers, our teach assistant and our friend in our class about the helping us, make this project, this presentation be done.

### References

[1] Github repository: Wavencoder - a python library for encoding raw audio with pytorch backend.

[2] Wav2vec 2.0: Learning the structure of speech from raw audio.

[3] Juan M. Coria, Hervé Bredin, Sahar Ghannay, and Sophie Rosset. A comparison of metric learning
loss functions for end-to-end speaker verification, 2020.

[4] Juan M. Coria, Hervé Bredin, Sahar Ghannay, and Sophie Rosset. Github repository: Companion
repository for the paper "a comparison of metric learning loss functions for end-to-end speaker
verification" published at slsp 2020, 2020.

[5] Github Repository: [Keras (tensorflow) implementation of SincNet](https://github.com/grausof/keras-sincnet) (Mirco Ravanelli, Yoshua Bengio, by Francesco Grauso, Evans Kiplagat

[6] Andy T. Liu, Shu-wen Yang, Po-Han Chi, Po-chun Hsu, and Hung-yi Lee. Mockingjay: Unsuper-
vised speech representation learning with deep bidirectional transformer encoders. ICASSP 2020 -
2020 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), May
2020.

[7] Son T. Nguyen, Viet D. Lai, Quyen Dam-Ba, Anh Nguyen-Xuan, and Cuong Pham. Vietnamese
speaker authentication using deep models. In Proceedings of the Ninth International Symposium
on Information and Communication Technology, SoICT 2018, page 177–184, New York, NY, USA,
2018. Association for Computing Machinery.

[8] Santiago Pascual, Mirco Ravanelli, Joan Serrà, Antonio Bonafonte, and Yoshua Bengio. Learning
problem-agnostic speech representations from multiple self-supervised tasks, 2019.

[9] Github Repository: [SincNet original code written in PyTorch by the autor](https://github.com/mravanelli/SincNet) - Mirco Ravanelli and Yoshua Bengio, 2019

[10] Mirco Ravanelli, Yoshua Bengio, “Speaker Recognition from raw waveform with SincNet” [Arxiv](https://arxiv.org/abs/1808.00158), 2019

[11] Steffen Schneider, Alexei Baevski, Ronan Collobert, and Michael Auli. wav2vec: Unsupervised
pre-training for speech recognition, 2019.

[12] Ehsan Variani, Xin Lei, Erik McDermott, Ignacio Lopez Moreno, and Javier Gonzalez-Dominguez.
Deep neural networks for small footprint text-dependent speaker verification. In Proc. ICASSP,
2014.

[13] Jee weon Jung, Seung bin Kim, Hye jin Shim, Ju ho Kim, and Ha-Jin Yu. Improved rawnet with
feature map scaling for text-independent speaker verification using raw waveforms, 2020.

[14] [A brief Introduction to SincNet](https://www.youtube.com/watch?v=mXQBObRGUgk), Mirco Ravanelli
