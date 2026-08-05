# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu được cập nhật từ **0h ngày 01/08/2026 đến 16h ngày 05/08/2026**.

## Nguyên tắc cập nhật
- Giữ nguyên toàn bộ bố cục, logo VNPT, màu sắc, bộ lọc, bảng 22 địa bàn và popup chi tiết.
- Chỉ cập nhật số liệu từ file Excel mới.

## Nguồn dữ liệu

### Sheet `TH`
- Danh sách 229 Điểm ủy quyền
- Nhóm Pro, Plus, Basic
- Số lượng thuê bao
- Doanh thu
- PSSL và PSSL gói từ 70k

### Sheet `Đơn hàng`
- Cột M: Mã ĐUQ
- Cột AB: chỉ lấy trạng thái `Thành công`
- Cột AV: Số thuê bao
- Cột BA: Doanh thu từng thuê bao

## Tổng quan
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

- Đã tạo lại toàn bộ **Top 3 Nhóm Pro, Plus, Basic** trực tiếp từ sheet `TH`.
- Top 3 được xếp theo **Doanh thu bán hàng giảm dần**; nếu doanh thu bằng nhau thì ưu tiên **Số lượng thuê bao cao hơn**.
- Mỗi thẻ chỉ lấy đúng:
  - `Tên ĐUQ`
  - `Đơn vị` (Khu vực)
  - `Số lượng Thuê bao`
  - `Doanh thu bán hàng`
- Đã loại bỏ dữ liệu Top 3 cũ bị lưu tĩnh và gây hiển thị sai `113 TB`.
