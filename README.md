# BÀI THỰC HÀNH 6 – BÁO CÁO PHÂN TÍCH KẾT QUẢ HỌC TẬP
# Chủ đề: Tổng hợp kết quả học tập 30 sinh viên lớp Java cơ bản bằng AI.

### 1. Các Prompt sử dụng để xử lý dữ liệu
Prompt 1 – Đọc File 1: Danh sách sinh viên
```
Đọc file danh sách sinh viên. Trích xuất mã sinh viên,
họ tên và lớp thành bảng có cấu trúc.

Sử dụng mã sinh viên làm khóa định danh chính.
Kiểm tra mã sinh viên bị trùng hoặc thiếu.
```


Prompt 2 – Đọc File 2: Chuyên cần và bài tập
```
Đọc file điểm chuyên cần và bài tập.
Trích xuất mã sinh viên, họ tên, điểm chuyên cần
và điểm bài tập thành bảng.

Kiểm tra điểm thiếu, dữ liệu trùng và điểm ngoài
thang 0-10. Không tự điền dữ liệu còn thiếu.
```

Prompt 3 – Đọc File 3: Điểm giữa kỳ
```
Đọc file điểm giữa kỳ. Trích xuất mã sinh viên,
họ tên và điểm giữa kỳ.

Kiểm tra dữ liệu trùng, thiếu điểm và sai khác
họ tên. Không tự sửa hoặc suy đoán điểm.
```

Prompt 4 – Đọc File 4: Điểm cuối kỳ và nhận xét
```
Đọc file điểm cuối kỳ và nhận xét giảng viên.

Trích xuất mã sinh viên, họ tên, điểm cuối kỳ
và nhận xét.

Kiểm tra điểm thiếu, dữ liệu trùng và thông tin
không nhất quán.
```

### 2. Prompt đối chiếu dữ liệu
Đối chiếu dữ liệu từ 4 file theo mã sinh viên.

Tổng hợp các trường:
Mã SV, Họ tên, Chuyên cần, Bài tập,
Giữa kỳ, Cuối kỳ.

Tính điểm tổng kết theo công thức:
10% chuyên cần + 20% bài tập
+ 30% giữa kỳ + 40% cuối kỳ.

Phân loại:
- Đạt: từ 5,0 điểm.
- Chưa đạt: dưới 5,0 điểm.
- Thiếu dữ liệu: chưa đủ điểm để tính.

Phát hiện dữ liệu trùng, thiếu hoặc sai khác.
Không tự điền điểm và không suy đoán nguyên nhân.


### 3. Bảng kết quả tổng hợp 30 sinh viên

| Mã SV | Họ tên | CC | BT | GK | CK | Tổng kết | Kết quả |
|---|---|---|---|---|---|---|---|
| 001 | Nguyễn Minh Anh | 9 | 8 | 7 | 8 | 7,8 | Đạt |
| 002 | Trần Đức Long | 8 | 7 | 6 | 7 | 6,8 | Đạt |
| 003 | Lê Hoàng Nam | 10 | 9 | 8 | 8 | 8,4 | Đạt |
| 004 | Phạm Thu Hà | 9 | 8 | 7 | 6 | 7,0 | Đạt |
| 005 | Nguyễn Minh Anh | 8 | 9 | — | 9 | — | Thiếu DL |
| 006 | Vũ Quốc Bảo | 7 | 6 | 5 | 5 | 5,4 | Đạt |
| 007 | Đỗ Khánh Linh | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 008 | Hoàng Gia Huy | 10 | — | 9 | 9 | — | Thiếu DL |
| 009 | Bùi Ngọc Mai | 8 | 7 | 6 | 6 | 6,4 | Đạt |
| 010 | Phan Tuấn Kiệt | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 011 | Đặng Hải Yến | 7 | — | 5 | 4 | — | Thiếu DL |
| 012 | Ngô Thành Đạt | 8 | 7 | 6 | 6 | 6,4 | Đạt |
| 013 | Trịnh Bảo Ngọc | 10 | 9 | 8 | — | — | Thiếu DL |
| 014 | Đinh Quang Hưng | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 015 | Mai Phương Thảo | 8 | 7 | 6 | 6 | 6,4 | Đạt |
| 016 | Cao Nhật Minh | 7 | 6 | 5 | 5 | 5,4 | Đạt |
| 017 | Lý Thanh Tùng | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 018 | Dương Hà My | 8 | 7 | — | 6 | — | Thiếu DL |
| 019 | Hồ Anh Tuấn | 10 | 9 | 9 | 9 | 9,1 | Đạt |
| 020 | Võ Thùy Dung | 9 | 8 | 8 | 8 | 8,1 | Đạt |
| 021 | Nguyễn Hoàng Phúc | 8 | 7 | 6 | 6 | 6,4 | Đạt |
| 022 | Trần Ngọc Ánh | 7 | 6 | 5 | 5 | 5,4 | Đạt |
| 023 | Lê Minh Khang | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 024 | Phạm Quỳnh Chi | 10 | 9 | 8 | 8 | 8,4 | Đạt |
| 025 | Vũ Đức Anh | 8 | 7 | 6 | — | — | Thiếu DL |
| 026 | Đỗ Minh Châu | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 027 | Hoàng Tuấn Anh | 7 | 6 | 5 | 5 | 5,4 | Đạt |
| 028 | Bùi Khánh Vy | 8 | 7 | 6 | 6 | 6,4 | Đạt |
| 029 | Phan Gia Bảo | 9 | 8 | 7 | 7 | 7,4 | Đạt |
| 030 | Đặng Minh Trang | 10 | 9 | 9 | 9 | 9,1 | Đạt |

CC: Chuyên cần · BT: Bài tập · GK: Giữa kỳ · CK: Cuối kỳ · Thiếu DL: Thiếu dữ liệu. Mã SV trong bảng đã rút gọn phần tiền tố JAVA26.

### 4. Báo cáo thống kê kết quả

| Chỉ tiêu | Số lượng | Tỷ lệ |
|---|---:|---:|
| Tổng số sinh viên | 30 | 100% |
| Sinh viên đạt | 24 | 80% |
| Sinh viên chưa đạt | 0 | 0% |
| Sinh viên thiếu dữ liệu | 6 | 20% |

### 5. Danh sách các trường hợp bất thường

| Mã SV | File | Bất thường |
|---|---|---|
| JAVA260001 và JAVA260005 | File 1 | Trùng họ tên nhưng khác mã sinh viên |
| JAVA260008 | File 2 | Trùng bản ghi, điểm bài tập 9 và 5 |
| JAVA260011 | File 2 | Thiếu điểm bài tập |
| JAVA260005 | File 3 | Trùng bản ghi, điểm giữa kỳ 8 và 7; khác cách viết tên |
| JAVA260018 | File 3 | Thiếu điểm giữa kỳ |
| JAVA260013 | File 4 | Trùng bản ghi, điểm cuối kỳ 8 và 6 |
| JAVA260025 | File 4 | Thiếu điểm cuối kỳ |

Hướng xử lý:
- Đối chiếu lại dữ liệu gốc với giảng viên.
- Xác minh các bản ghi bị trùng.
- Bổ sung điểm còn thiếu sau khi có xác nhận.
- Không tự chọn điểm hoặc tự điền dữ liệu.
### 6. Báo cáo nhận xét tình hình học tập
Lớp Java cơ bản có tổng cộng 30 sinh viên. Sau khi tổng hợp dữ liệu từ 4 tài liệu, hệ thống xác định được 24 sinh viên có đủ thông tin để tính điểm tổng kết, chiếm 80% sĩ số lớp.

Trong số 24 sinh viên đủ dữ liệu, cả 24 sinh viên đều đạt học phần với điểm tổng kết từ 5,0 trở lên. Không có trường hợp nào được xác định là chưa đạt trong nhóm dữ liệu đầy đủ.

Tuy nhiên, quá trình xử lý phát hiện 6 trường hợp thiếu hoặc có dữ liệu điểm không thống nhất. Cụ thể, có sinh viên thiếu điểm bài tập, giữa kỳ hoặc cuối kỳ. Một số trường hợp xuất hiện nhiều bản ghi với điểm số khác nhau. Ngoài ra, có hai sinh viên trùng họ tên nhưng mang mã sinh viên khác nhau.

Những vấn đề này cho thấy dữ liệu đầu vào chưa hoàn toàn đồng nhất và cần được kiểm tra trước khi đưa ra kết luận cuối cùng.

Để đảm bảo tính chính xác, cần đối chiếu các bản ghi bất thường với tài liệu gốc và xác nhận lại với giảng viên. Không tự ý bổ sung điểm hoặc suy đoán nguyên nhân kết quả học tập.

Kết luận: Kết quả ban đầu cho thấy tình hình học tập của nhóm sinh viên có đủ dữ liệu khá tốt. Tuy nhiên, báo cáo chưa thể xem là kết quả cuối cùng của toàn lớp cho đến khi 6 trường hợp còn thiếu dữ liệu được xác minh.
