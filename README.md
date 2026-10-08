## 1\. Đề xuất 2 cách thực hiện

* Cách 1: Sử dụng Giao diện đồ họa (GUI): Mở File Explorer, thực hiện thao tác click chuột phải \-\> *New Folder* lặp đi lặp lại 50 lần cho từng thư mục (Quản lý bàn, Quản lý kho, Menu, v.v.).  
* Cách 2: Sử dụng Giao diện dòng lệnh (CLI): Viết một câu lệnh PowerShell hoặc Bash duy nhất để hệ thống tự động sinh ra toàn bộ cấu trúc thư mục ngay lập tức.

  ## 2\. Bảng so sánh Ưu điểm / Nhược điểm giữa GUI và CLI

| Tiêu chí | Giao diện đồ họa (GUI) | Giao diện dòng lệnh (CLI) |
| ----- | ----- | ----- |
| Tốc độ thực hiện | Rất chậm: Mất nhiều thời gian click chuột thủ công 50 lần, dễ bị mỏi tay và quá tải trong giới hạn 1 giờ. | Cực kỳ nhanh: Chỉ mất vài giây để tạo hàng loạt thư mục cùng lúc. |
| Khả năng lặp lại / Tự động hóa | Thấp: Không thể tự động hóa, nếu sai sót hoặc cần nhân bản sang 100 chi nhánh phải làm lại từ đầu bằng tay. | Cao: Có thể lưu lại thành file script để chạy lại bất cứ lúc nào hoặc tự động hóa cho hàng loạt máy chủ chi nhánh. |
| Mức độ dễ học cho người mới | Cao: Thân thiện, trực quan, dễ làm quen ngay từ lần đầu nhìn thấy. | Thấp hơn: Người dùng cần phải ghi nhớ cú pháp câu lệnh cơ bản. |

  ## 3\. Chốt giải pháp và Giải thích lý do cứu sống dự án

* Giải pháp chốt: Lựa chọn Cách 2 (CLI \- Dòng lệnh).  
* Lý do cứu sống dự án: Với áp lực thời gian chỉ có 1 giờ để tạo cấu trúc cho hệ thống 100 chi nhánh mới, việc dùng GUI (click chuột 50 lần) cực kỳ rủi ro: dễ bị nhầm lẫn tên, thiếu sót thư mục do thao tác thủ công và không kịp tiến độ. CLI giúp tự động hóa toàn bộ công việc trong vài giây với độ chính xác tuyệt đối, đảm bảo bàn giao đúng hạn.

  ## 4\. Thiết kế thao tác lệnh CLI mẫu

Lệnh PowerShell để tạo nhanh 3 thư mục mẫu (`Ban`, `Kho`, `Menu`) trong một dòng duy nhất:

PowerShell

* mkdir Ban, Kho, Menu  
    
* 

