# Chương trình đồng hành cùng Điểm ủy quyền

Phiên bản dữ liệu cập nhật đến **16h ngày 04/08/2026**.

## Nguyên tắc cập nhật
- Giữ nguyên toàn bộ bố cục, màu sắc, logo VNPT, hình ảnh và chức năng của bảng chốt.
- Chỉ cập nhật dữ liệu từ file Excel mới.

## Nguồn dữ liệu
### Sheet `TH`
- Thông tin ĐUQ
- Nhóm Pro, Plus, Basic
- Số lượng thuê bao
- Doanh thu
- PSSL và PSSL gói từ 70k

### Sheet `Đơn hàng`
- Cột M: Mã ĐUQ
- Cột AB: chỉ lấy trạng thái `Thành công`
- Cột AV: Số thuê bao
- Cột BA: Doanh thu từng thuê bao

## Tổng quan dữ liệu
- Tổng ĐUQ: **229**
- Nhóm Pro: **27**
- Nhóm Plus: **30**
- Nhóm Basic: **172**
- Tổng thuê bao: **218**
- Tổng doanh thu: **14,968,000 đồng**
- ĐUQ có PSSL: **91**
- ĐUQ chưa PSSL: **138**
- ĐUQ PSSL gói từ 70k: **42**
- Tổng đơn hàng thành công: **225**

## Cập nhật GitHub Pages
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.

- Bổ sung cột **Tổng thuê bao** ngay sau cột **PSSL ≥70k** trong bảng 22 địa bàn.
- Bổ sung cột **Tổng doanh thu** ngay sau cột **Tổng thuê bao**.
- **Tổng thuê bao** là tổng số thuê bao của toàn bộ ĐUQ thuộc địa bàn.
- **Tổng doanh thu** là tổng doanh thu bán hàng của toàn bộ ĐUQ thuộc địa bàn.
- Có thể bấm vào hai cột mới để mở danh sách ĐUQ chi tiết:
  - Tổng thuê bao: sắp xếp theo thuê bao từ cao xuống thấp.
  - Tổng doanh thu: sắp xếp theo doanh thu từ cao xuống thấp.
- Hai chỉ tiêu mới cũng được bổ sung vào droplist **Xem nhanh theo chỉ tiêu**.
