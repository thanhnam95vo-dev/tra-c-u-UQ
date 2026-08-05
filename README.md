# Chương trình đồng hành cùng Điểm ủy quyền

Phiên bản dữ liệu cập nhật đến **16h ngày 05/08/2026**.

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

- Trong danh sách **ĐUQ có PSSL**, **ĐUQ chưa PSSL** và **PSSL gói từ 70k**, bổ sung droplist lọc theo 22 khu vực.
- Trong bảng **Theo dõi 22 địa bàn**, bổ sung cột cảnh báo **ĐUQ chưa PSSL**.
- Bấm vào số lượng **ĐUQ chưa PSSL** của một địa bàn sẽ:
  - Chuyển sang danh sách ĐUQ chưa PSSL.
  - Tự động chọn đúng khu vực trong droplist.
  - Hiển thị nhanh danh sách ĐUQ cần hỗ trợ.

- Đã sửa lỗi lệch cột trong bảng 22 địa bàn.
- Nguyên nhân: phần dữ liệu đã có cột **Chưa PSSL** nhưng tiêu đề bảng chưa có, làm toàn bộ các cột phía sau bị dịch sai.
- Thứ tự cột chuẩn hiện tại:
  1. XH
  2. Địa bàn
  3. Tổng ĐUQ
  4. PSSL
  5. Chưa PSSL
  6. Tỷ lệ PSSL
  7. PSSL ≥70k
  8. Tổng thuê bao
  9. Tổng doanh thu
  10. ≥5 SIM
  11. ≥10 SIM
  12. ≥20 SIM
  13. DT <500K
  14. DT ≥500K
  15. DT ≥1 triệu
  16. DT ≥2 triệu
