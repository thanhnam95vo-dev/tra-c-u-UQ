# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu cập nhật từ 0h ngày 01/08/2026 đến 7h30 ngày 19/08/2026.

## Tổng quan đã đối chiếu
- Tổng ĐUQ: **266**
- Tổng thuê bao PTM: **1.111**
- Thuê bao PTM từ 70k: **623**
- Tổng doanh thu: **114.629.000 đồng**
- ĐUQ có PSSL: **210**
- ĐUQ chưa PSSL: **56**

## Nguồn và mốc chốt
- Danh mục ĐUQ lấy từ sheet **TH**.
- Đơn hàng lấy từ sheet **Đơn hàng**.
- Chỉ lấy đơn hàng **Thành công**, có thời gian đăng ký thành công từ **0h 01/08/2026 đến 7h30 ngày 19/08/2026** cho phần Tra cứu ĐUQ.
- Thuê bao PTM lấy theo cột chốt **BB**; thuê bao PTM từ 70k theo cột **BC**; doanh thu theo cột **BA**.
- Phần **Tri ân** được tính riêng theo dữ liệu ngày **18/08/2026**.
- Phần **Tra cứu ĐUQ** được tính cộng dồn từ **01/08/2026 đến 19/08/2026**.

## Các lỗi đã sửa
- Bỏ phần **Tổng quan** và **Theo dõi 22 địa bàn** khỏi phiên bản dành cho Điểm ủy quyền.
- Khi mở file, trang mặc định vào phần **Tri ân 18/08**.
- Phần **Tra cứu ĐUQ** đã đồng bộ lại số thuê bao, thuê bao từ 70k, doanh thu và danh sách thuê bao theo dữ liệu từ 01/08 đến 19/08.
- Chi tiết thuê bao hiển thị đầy đủ **ngày và giờ đăng ký thành công**.
- Phần **Xếp hạng và giải thưởng** đã được chuẩn hóa theo 2 trạng thái:
  - Nếu đủ điều kiện: hiển thị **Đủ điều kiện**, thứ hạng, tên giải và mức tiền thưởng.
  - Nếu chưa đủ điều kiện: hiển thị **Chưa đủ điều kiện**, thứ hạng `—`, xếp loại **Chưa đủ điều kiện**, mức tiền thưởng **0 đồng**.
- Dòng trạng thái đầu trang đã đổi thành: **Dữ liệu cập nhật từ 0h ngày 01/08/2026 đến 7h30 ngày 19/08/2026**.

## Chương trình Tri ân ngày 18/08/2026
- 01 Giải đặc biệt: **500.000 đồng**.
- 01 Giải nhất: **300.000 đồng**.
- 03 Giải nhì: **200.000 đồng/giải**.
- 05 Giải ba: **100.000 đồng/giải**.
- Xếp hạng theo doanh thu ngày **18/08/2026** giảm dần.
- Điều kiện:
  - Giải đặc biệt: doanh thu từ **3.000.000 đồng**.
  - Giải nhất: doanh thu từ **2.000.000 đồng**.
  - Giải nhì: doanh thu từ **1.000.000 đồng**.
  - Giải ba: doanh thu từ **500.000 đồng**.
- Dữ liệu Tri ân chỉ tính trong **ngày 18/08/2026**.

### Kết quả xếp hạng chính thức
| Hạng | Điểm ủy quyền | Địa bàn | Thuê bao | Doanh thu | Giải thưởng |
|---:|---|---|---:|---:|---|
| 1 | CỬA HÀNG VINAPHONE VĂN THÀNH 2 | Kiến Tường | 11 | 3.120.000đ | Giải đặc biệt – 500.000đ |
| 2 | CÔNG TY TNHH TMDV VIỄN THÔNG HÙNG PHÁT | Cần Đước | 19 | 3.000.000đ | Giải nhất – 300.000đ |
| 3 | CỬA HÀNG Kì Ân | Tân Ninh | 1 | 1.000.000đ | Giải nhì – 200.000đ |
| 4 | CỬA HÀNG Gia Tường | Tân Ninh | 1 | 790.000đ | Giải ba – 100.000đ |
| 5 | CỬA HÀNG VINAPHONE CÁT PHƯỢNG | Cần Đước | 1 | 770.000đ | Giải ba – 100.000đ |
| 6 | Điểm Ủy quyền TÔ HỒNG BÍCH LIỄU | Cần Giuộc | 6 | 750.000đ | Giải ba – 100.000đ |

**Đánh giá:** Có **6 ĐUQ đủ điều kiện nhận giải** trong dữ liệu ngày 18/08/2026. Chưa lấp đủ toàn bộ số lượng giải theo cơ cấu chương trình vì các Điểm ủy quyền còn lại chưa đạt ngưỡng doanh thu tối thiểu tương ứng.

## Tra cứu Điểm ủy quyền
- Phạm vi dữ liệu: từ **01/08/2026 đến 19/08/2026**.
- Tổng ĐUQ: **266**.
- Tổng thuê bao PTM: **1.111**.
- Thuê bao PTM từ 70k: **623**.
- Tổng doanh thu: **114.629.000 đồng**.
- Khi bấm vào từng ĐUQ, hệ thống hiển thị danh sách thuê bao đăng ký thành công theo thời gian mới nhất trước.
- Mỗi thuê bao có số điện thoại, doanh thu và ngày giờ đăng ký thành công.
- Phần **Xếp hạng và giải thưởng** trong chi tiết ĐUQ phản ánh kết quả chương trình Tri ân ngày **18/08/2026**.

## Cập nhật GitHub
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.
