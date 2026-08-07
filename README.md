# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu cập nhật từ **0h ngày 01/08/2026 đến 16h30 ngày 07/08/2026**.

## Tổng quan
- Tổng ĐUQ: **229**
- Nhóm Pro: **27**
- Nhóm Plus: **30**
- Nhóm Basic: **172**
- Tổng thuê bao PTM: **346**
- Thuê bao PTM từ 70k: **154**
- Tổng doanh thu: **28,209,000 đồng**
- ĐUQ có PSSL: **117**
- ĐUQ chưa PSSL: **112**
- ĐUQ PSSL gói từ 70k: **62**

## ĐUQ chưa PSSL theo phân loại
- ĐUQ trước năm 2026: **59**
- ĐUQ trong năm 2026: **18**
- ĐUQ mới: **35**

## Đối chiếu dữ liệu
- Không có ID ĐUQ trống: **Đạt**
- Không có ID ĐUQ trùng: **Đạt**
- Đủ 22 địa bàn: **Đạt**
- Tổng thuê bao theo 22 địa bàn khớp sheet TH: **Đạt**
- Tổng TB từ 70k theo 22 địa bàn khớp sheet TH: **Đạt**
- Tổng doanh thu theo 22 địa bàn khớp sheet TH: **Đạt**
- Đơn hàng thành công map đúng ĐUQ: **346**
- Thuê bao từ 70k trong sheet Đơn hàng: **154**

## Tri ân ngày 07/08/2026
- Thời gian xét: **0h đến 16h30 ngày 07/08/2026**
- Đơn hàng thành công của ĐUQ trong ngày: **67**
- Điều kiện: **Doanh thu ngày 07/8 từ 200.000đ trở lên**
- ĐUQ đủ điều kiện: **11**
- Vị trí giải còn trống: **2**
- Click từng ĐUQ để xem SIM/số thuê bao, thời gian thành công và doanh thu ngày 07/8.

## Trường dữ liệu sử dụng
- Sheet `TH`: dữ liệu tổng hợp ĐUQ.
- Sheet `Đơn hàng`: `M - Mã HRM CTV/Đại lý`, `AA - Ngày ĐH thành công`, `AB - Trạng thái`, `AV - Số thuê bao`, `BA - Doanh thu chốt`, `BB - Thuê bao chốt`, `BC - Thuê bao từ 70k`.
- Chỉ lấy `AB = Thành công`, `BB > 0`; map `M` với `ID điểm bán` ở sheet `TH`.

## Cập nhật GitHub
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.


## Sửa lỗi tra cứu
- Khôi phục danh sách trường tìm kiếm `FIELDS` bị thiếu trong JavaScript.
- Thanh tìm kiếm chung có thể tìm theo: Tên ĐUQ, ID điểm bán, HRM điểm bán, Đơn vị, Nhân viên hỗ trợ, SĐT nhân viên hỗ trợ, Bảng thi đấu và Trạng thái ĐUQ.
- Khi bấm menu **Tra cứu ĐUQ**, danh sách toàn bộ ĐUQ được hiển thị lại bình thường; nhập từ khóa sẽ lọc tức thời.
- Giữ nguyên dữ liệu cập nhật đến **16h30 ngày 07/08/2026** và toàn bộ chức năng khác.
