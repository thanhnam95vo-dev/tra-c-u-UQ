# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu cập nhật từ **0h ngày 01/08/2026 đến 16h ngày 06/08/2026**.

## Tổng quan
- Tổng ĐUQ: **229**
- Nhóm Pro: **27**
- Nhóm Plus: **30**
- Nhóm Basic: **172**
- Tổng thuê bao PTM: **264**
- Thuê bao PTM từ 70k: **104**
- Tổng doanh thu: **18,497,000 đồng**
- ĐUQ có PSSL: **101**
- ĐUQ chưa PSSL: **128**
- ĐUQ PSSL gói từ 70k: **47**

## ĐUQ chưa PSSL theo phân loại
- ĐUQ trước năm 2026: **70**
- ĐUQ trong năm 2026: **20**
- ĐUQ mới: **38**

## Đối chiếu dữ liệu
- Không có ID ĐUQ trống: **Đạt**
- Không có ID ĐUQ trùng: **Đạt**
- Đủ 22 địa bàn: **Đạt**
- Tổng thuê bao theo 22 địa bàn khớp sheet TH: **Đạt**
- Tổng TB từ 70k theo 22 địa bàn khớp sheet TH: **Đạt**
- Tổng doanh thu theo 22 địa bàn khớp sheet TH: **Đạt**
- Đơn hàng thành công map đúng ĐUQ: **264**
- Thuê bao từ 70k trong sheet Đơn hàng: **104**
- Mã đơn hàng thành công không tồn tại trong sheet TH: **8**

## Cập nhật GitHub
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.

- Bổ sung **Ngày đăng ký thành công** cho từng số thuê bao trong popup.
- Nguồn dữ liệu: sheet `Đơn hàng`, cột `AA - Ngày ĐH thành công`.
- Chỉ lấy các dòng có cột `AB = Thành công`.
- Danh sách thuê bao được sắp xếp theo ngày đăng ký thành công mới nhất đến cũ nhất.
- Định dạng hiển thị: `dd/MM/yyyy HH:mm`; nếu không có giờ thì hiển thị `dd/MM/yyyy`.
- Áp dụng cho cả tab **Tất cả TB PTM** và **TB PTM từ 70k**.
