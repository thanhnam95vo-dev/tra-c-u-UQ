# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu cập nhật từ **0h ngày 01/08/2026 đến 23h59 ngày 07/08/2026**.

## Tổng quan
- Tổng ĐUQ: **253**
- Nhóm Pro: **27**
- Nhóm Plus: **30**
- Nhóm Basic: **196**
- Tổng thuê bao PTM: **374**
- Thuê bao PTM từ 70k: **173**
- Tổng doanh thu: **31.199.000 đồng**
- ĐUQ có PSSL: **126**
- ĐUQ chưa PSSL: **127**
- ĐUQ PSSL gói từ 70k: **66**

## ĐUQ chưa PSSL theo phân loại
- ĐUQ trước năm 2026: **57**
- ĐUQ trong năm 2026: **18**
- ĐUQ mới: **52**

## Tri ân ngày 07/08/2026
- Nguồn: sheet `Đơn hàng`.
- Chỉ lấy dòng `AB = Thành công` và `BB - Thuê bao chốt > 0`.
- Mã ĐUQ: cột `M - Mã HRM CTV/Đại lý`.
- Ngày thành công: cột `AA - Ngày ĐH thành công`.
- Số thuê bao: cột `AV - Số thuê bao`.
- Doanh thu: cột `BA - Doanh thu chốt`.
- Thuê bao từ 70k: cột `BC - Thuê bao từ 70k`.
- Đơn hàng thành công ngày 07/8: **94**.
- ĐUQ đạt điều kiện doanh thu ≥200.000đ: **17**.
- Số vị trí giải: **13**; còn trống: **0**.
- Xếp hạng theo doanh thu ngày 07/8 giảm dần; nếu bằng doanh thu, ưu tiên số thuê bao cao hơn.
- Khi click ĐUQ nhận giải, hiển thị SIM/thuê bao, thời gian thành công và doanh thu từng SIM trong ngày 07/8.

## Theo dõi 22 địa bàn — đã fix
- Đã khôi phục biến dữ liệu `AREA_STATS` từ dữ liệu sheet `TH`.
- Mục **Theo dõi và xếp hạng 22 địa bàn** hiển thị đủ số liệu theo từng địa bàn.
- Tổng quan gồm: Tổng ĐUQ, PSSL, chưa PSSL, tỷ lệ PSSL và phân loại chưa PSSL.
- Thuê bao & Doanh thu gồm: tổng TB PTM, TB từ 70k, các ngưỡng số SIM và các ngưỡng doanh thu.
- Cột Địa bàn tiếp tục cố định khi kéo ngang; header và dòng tổng giữ cố định khi cuộn.

## Tra cứu & chi tiết
- Thanh tìm kiếm tra cứu theo: Tên ĐUQ, ID điểm bán, HRM, đơn vị, nhân viên hỗ trợ, SĐT hỗ trợ, bảng thi đấu và trạng thái ĐUQ.
- Danh sách ĐUQ chưa PSSL có dropdown lọc theo 22 địa bàn.
- Popup ĐUQ hiển thị danh sách thuê bao phát triển mới và thuê bao từ 70k theo đơn hàng thành công.

## Đối chiếu dữ liệu
- ID ĐUQ hợp lệ, không trùng trong dashboard: **253**.
- Đủ 22 địa bàn trong module theo dõi: **Đạt**.
- Tổng TB PTM theo sheet TH: **374**.
- Tổng TB từ 70k theo sheet TH: **173**.
- Tổng doanh thu theo sheet TH: **31.199.000 đồng**.

## Cập nhật GitHub
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.
