# Chương trình đồng hành cùng Điểm ủy quyền

Dữ liệu cập nhật đến **12h51 ngày 06/08/2026**.

## Nội dung bổ sung
- Phân loại ĐUQ:
  - ĐUQ trước năm 2026: **156**
  - ĐUQ trong năm 2026: **28**
  - ĐUQ mới: **45**
- Tổng thuê bao PTM: **252**
- Tổng thuê bao PTM từ 70k: **99**
- Tổng doanh thu: **16,532,000 đồng**

## Chức năng
- Bấm vào từng thẻ phân loại để mở danh sách ĐUQ tương ứng.
- Hiển thị phân loại ĐUQ trong danh sách và popup chi tiết.
- Thêm KPI **Thuê bao PTM từ 70k**.
- Thêm chỉ tiêu **Tổng TB PTM từ 70k** vào bộ lọc nhiều lựa chọn.
- Thêm cột **Tổng TB PTM từ 70k** trong bảng Theo dõi 22 địa bàn.
- Dòng tổng và thanh trạng thái của bảng 22 địa bàn có tổng TB PTM từ 70k.
- Các số liệu tiếp tục có thể bấm để xem danh sách chi tiết.

## Cập nhật GitHub
Upload đè `index.html` và `README.md`, sau đó chọn **Commit changes**.

- Tất cả nút **TB PTM từ 70k** có thể bấm để xem danh sách số thuê bao chi tiết.
- Danh sách chi tiết được lấy từ sheet `Đơn hàng`:
  - Cột M: Mã ĐUQ
  - Cột AB: trạng thái `Thành công`
  - Cột AV: số thuê bao
  - Cột BA: doanh thu thuê bao
  - Cột BC: đánh dấu `Thuê bao từ 70k = 1`
- Popup có hai tab:
  - Tất cả TB PTM
  - TB PTM từ 70k
- Tổng thuê bao từ 70k trong chi tiết: **99**

- Đã sửa cách xử lý dữ liệu tab thuê bao để JavaScript chạy ổn định trên GitHub Pages và điện thoại.

- Chia bảng **Theo dõi 22 địa bàn** thành 2 menu:
  1. **Tổng quan**: SL ĐUQ, ĐUQ PSSL, Tỷ lệ PSSL, Chưa PSSL và phân loại chưa PSSL theo ĐUQ trước năm 2026, trong năm 2026, ĐUQ mới.
  2. **Thuê bao & Doanh thu**: Tổng TB PTM, TB PTM từ 70k, các ngưỡng SIM và doanh thu.
- Bổ sung chỉ tiêu:
  - SL ĐUQ dưới 5 SIM
  - SL ĐUQ từ 30 SIM
  - SL ĐUQ doanh thu từ 3 triệu
- Dòng tổng và tất cả số liệu vẫn có thể bấm xem danh sách chi tiết.

- Thêm droplist **Bộ lọc chỉ tiêu** đặt cạnh droplist **22 địa bàn**.
- Danh sách chỉ tiêu tự thay đổi theo menu:
  - Tổng quan
  - Thuê bao & Doanh thu
- Khi chọn một chỉ tiêu:
  - Chỉ hiển thị cột chỉ tiêu đó.
  - Chỉ hiển thị địa bàn có giá trị lớn hơn 0.
  - Tự sắp xếp từ cao xuống thấp.
- Có thể kết hợp đồng thời bộ lọc chỉ tiêu và bộ lọc địa bàn.

- Trong mục **ĐUQ chưa PSSL**, bổ sung 4 menu lọc nhanh:
  - Tất cả ĐUQ chưa PSSL: **130**
  - ĐUQ trước năm 2026: **71**
  - ĐUQ trong năm 2026: **20**
  - ĐUQ mới: **39**
- Có thể kết hợp menu phân loại với droplist 22 khu vực.
- Khi bấm từng menu, danh sách và các chỉ số tổng hợp được cập nhật theo đúng phân loại.

- Làm rõ danh sách ĐUQ chưa PSSL theo 3 nhóm:
  - ĐUQ trước năm 2026
  - ĐUQ phát triển trong năm 2026
  - ĐUQ mới
- Khi chọn từng nhóm, tiêu đề hiển thị rõ nhóm đang xem và số lượng điểm.
- Danh sách bên dưới thể hiện chính xác tên từng Điểm ủy quyền thuộc nhóm đó.

- Di chuyển các menu phân loại ĐUQ chưa PSSL lên ngay dưới tiêu đề danh sách.
- Bốn menu gồm:
  - Tất cả ĐUQ chưa PSSL
  - ĐUQ trước năm 2026
  - ĐUQ trong năm 2026
  - ĐUQ mới
- Mỗi menu hiển thị số lượng tổng và có thể kết hợp với bộ lọc 22 khu vực.

- Chỉnh mục **ĐUQ chưa PSSL** thành đúng 3 menu ngang:
  - ĐUQ trước năm 2026
  - ĐUQ trong năm 2026
  - ĐUQ mới
- Xóa dòng **Đang xem...**
- Không hiển thị nút Tất cả trong thanh menu.
- Khi bấm lại menu đang chọn, hệ thống quay về danh sách tất cả ĐUQ chưa PSSL.
- Vẫn giữ nguyên bộ lọc 22 khu vực và các chức năng xem chi tiết.

- Sửa lỗi 3 menu phân loại chưa hiển thị trong mục **ĐUQ chưa PSSL**.
- Nguyên nhân: khối menu vẫn còn trạng thái ẩn `display:none`.
- Menu giờ được bật/tắt theo đúng chế độ:
  - Hiện khi mở ĐUQ chưa PSSL.
  - Ẩn ở các danh sách khác.
