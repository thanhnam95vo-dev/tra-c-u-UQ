# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu từ **0h ngày 01/08/2026 đến 23h59 ngày 05/08/2026**.

## Nguồn số liệu chính

### Sheet `TH`
Toàn bộ Dashboard, Top 3, PSSL và bảng 22 địa bàn lấy trực tiếp từ sheet `TH`.

- Tổng ĐUQ: **229**
- Nhóm Pro: **27**
- Nhóm Plus: **30**
- Nhóm Basic: **172**
- Tổng thuê bao: **238**
- Tổng doanh thu: **15,928,000 đồng**
- ĐUQ có PSSL: **94**
- ĐUQ chưa PSSL: **135**
- ĐUQ PSSL gói từ 70k: **45**

### Sheet `Đơn hàng`
Chi tiết thuê bao được lấy theo:
- Cột M: Mã ĐUQ
- Cột AB: chỉ lấy trạng thái `Thành công`
- Cột AV: Số thuê bao
- Cột BA: Doanh thu từng thuê bao

## Kết quả đối chiếu

- Không có ID ĐUQ trống trong sheet `TH`.
- Không có ID ĐUQ trùng trong sheet `TH`.
- Đủ đúng **22 địa bàn**.
- Tổng số ĐUQ, PSSL, PSSL ≥70k, thuê bao và doanh thu cộng theo 22 địa bàn đều khớp 100% với sheet `TH`.
- Có **238** đơn hàng thành công map đúng mã ĐUQ trong sheet `TH`.
- Tổng doanh thu các đơn hàng map đúng: **15,928,000 đồng**.
- Hai giá trị này khớp chính xác với **238 thuê bao** và **15,928,000 đồng** trên sheet `TH`.
- Có **7** đơn hàng thành công thuộc **6 mã** không tồn tại trong danh sách ĐUQ của sheet `TH`; các đơn này không được đưa vào Dashboard và popup ĐUQ để tránh sai lệch.

Mã không tồn tại trong `TH`: `KBH001959, KBH028071_201, KBH173395, KBH173524, KBH199496, KBH335731`.

## Quy tắc Top 3

Top 3 của từng nhóm lấy đúng từ sheet `TH` theo thứ tự:
1. Doanh thu bán hàng giảm dần.
2. Nếu doanh thu bằng nhau, ưu tiên số lượng thuê bao cao hơn.
3. Hiển thị đúng Tên ĐUQ, Khu vực, Số lượng thuê bao và Doanh thu.

## Cập nhật GitHub Pages

Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.
