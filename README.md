# BTL-Xulyhinhanh

Giới thiệu

Dự án này tập trung vào việc nhận diện 31 cử chỉ tay sử dụng mạng nơ-ron tích chập (CNN), phục vụ cho ứng dụng như giao tiếp bằng ngôn ngữ ký hiệu (sign language), điều khiển thiết bị thông minh, và hỗ trợ người khiếm thính.

Hệ thống nhận diện bao gồm:
 • 26 chữ cái trong bảng chữ cái ngôn ngữ ký hiệu (tương ứng với a-z).
 • 5 ký hiệu đặc biệt/thao tác ngôn ngữ như: dấu mũ, hỏi, sắc, huyền, nặng.

Phương pháp
 • Tiền xử lý ảnh: Chuyển ảnh về thang xám, resize về 64x64, chuẩn hóa giá trị pixel.
 • Kiến trúc CNN: 3 lớp tích chập + pooling, kết nối dense, softmax output.
 • Huấn luyện mô hình: Tập dữ liệu được phân chia theo từng cử chỉ tay, huấn luyện trên TensorFlow/Keras.
 • Đánh giá mô hình: Accuracy > 90% trên tập kiểm thử.

Tập dữ liệu
 • Gồm 31 lớp tương ứng với mỗi cử chỉ.
 • Mỗi lớp chứa 200–500 ảnh, định dạng ảnh chụp bàn tay từ camera.
 • Dữ liệu có thể thu thập thủ công hoặc sử dụng bộ dữ liệu sẵn có (ví dụ: ASL Dataset, tự thu thập qua webcam).

Ứng dụng
 • Nhận diện cử chỉ tay từ webcam thời gian thực.
 • Hiển thị ký tự tương ứng trên màn hình.
 • Ứng dụng trong lớp học, công nghệ hỗ trợ, và hệ thống tương tác người–máy.

# Ảnh minh hoạ

![z6678974753318_b45fde2fe2ba61e6f4b070925a5e8eb1](https://github.com/user-attachments/assets/409901ae-493f-4b8f-bbc1-9a0210b4d144)
![z6678974748540_826f7b6186ba3d81cc180d84c8b62068](https://github.com/user-attachments/assets/90d9a7dd-00b9-45cd-861b-6c483585088e)
![z6678974768341_455d6e096924dbebc0ca055babb808cf](https://github.com/user-attachments/assets/9452be4f-7640-4abe-a3b3-15c5d48c3b91)
![z6678974761900_6861be14217fa1adb1d1425ebaf17bc7](https://github.com/user-attachments/assets/a4444b21-2e3a-4e18-9fc9-afbd449d51ef)
![z6678974760734_d2cc802c8adce610ba35598943dfff23](https://github.com/user-attachments/assets/5ed0e7b4-fa36-4d04-b038-a211f62743f7)
