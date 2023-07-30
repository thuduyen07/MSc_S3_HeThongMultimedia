# MSc_S3: Hệ Thống Multimedia

## 300723
### Yêu cầu môn học:
Đồ án cuối kỳ:
- Làm ứng dụng
- Minh hoạ systems và có thể chạy từng phần (từng module)

Kiểm tra cuối kỳ: 
- Làm seminar =))

### Reference
Computer Vision 
- MIT Spring 2023 course: http://6.8300.csail.mit.edu/sp23/schedule.html

Computational Photography
- UIUC Fall 2022: https://courses.engr.illinois.edu/cs445/fa2022/

Information Retrieval:

Multimedia Forensics: 
- Bài toán: Out-of-context

Giới thiệu dataset: 
- Place 365 (MIT): dùng để tạo video, lồng nhạc dô =))

Stable Diffusion => synthesize



### Nội dung chi tiết
#### Giới thiệu Xử lý ảnh
Một số ứng dụng:
 - 
 - visual creation
 - impainting

Electromagnetic spectrum:
- màu mà ta gọi tên là chỗ có nhiều photon bước sóng tương ứng -- Hue (H)
- màu bị trộn lẫn bởi những cái khác -- Saturation (S)
- Tổng số lượng photon tại đó -- Lightness (L), Intensity (I), Value (V)
Hệ màu:
- RGB
- HSV/HSL/HSI

Filters
- Sensor array
I = (R + G + B)/3

I = 0.3R + 0.59G + 0.11B

Pixel privacy => MediaEval: Đánh lừa các classifier của deeplearning =))

Filter vs. Warp
- filter: h(f(x)), có 2 dạng filter:
    1. Spatial filter
    2. Frequency 
- Một số filter:
    - box filter: dùng để smoothing (triệt tiêu/giảm sự khác biệt quá đáng của điểm đang xét với các điểm xung quanh)
    - median filter: tính trung bình cộng làm lan truyền sự khác biệt sang các điểm xung. Vì thế, ta dùng median, đầu tiên ta sắp lại theo tăng dần hoặc giảm dần điểm đang xét và các điểm lân cận và loại bỏ điểm oulier nếu có => thường dùng để lại nhiễu cho các ảnh bị muối tiêu
    - linear filter
    - sharpening filter
    - sobel filter: lọc biên cạnh (ngang/dọc), thằng nào gần nghe nó nhiều hơn =))
    - prewitt filter: lấy phiếu bầu đều nhau
    - gaussian filter: làm mượt dữ liệu, nghe thằng gần hơn nhưng với phân phối gauss 

Ảnh làm mờ (trơn): 
high pass: ảnh gốc trừ ảnh mờ -- còn lại 
high-boost: ảnh còn nội dung, chỉ làm sắc nét, tăng cường nét chi tiết trong ảnh --> dùng cho tiền xử lý dữ liệu trước khi đưa vào các thuật toán deep learning
    
- warp: f(h(x))

Giới thiệu một số project trong UIUC course:
- project 1: Hybird images (trộn ảnh)
- project 2: Image quilting
- project 3: gradient domain fus 
- camouflage object detection

vector gradient:
- 

saliency detection

seam carving: dùng để resize ảnh, dùng khá ổn trên ảnh phong cảnh, tuy nhiên không thực sự tốt khi có ảnh mặt người -> dùng penalty để đánh phạt các vùng không được động đến

- Tuần sau học cn 8h C22