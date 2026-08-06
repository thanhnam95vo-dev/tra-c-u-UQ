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

- Sửa lỗi cột **Địa bàn** bị cắt tên khi kéo ngang.
- Cố định cột **XH** rộng 56px.
- Cố định cột **Địa bàn** rộng 190px.
- Tăng lớp hiển thị `z-index` để hai cột cố định luôn nằm trên các cột chỉ tiêu.
- Giữ nguyên dòng tổng và tiêu đề cố định.

- Thu gọn cột **XH** từ 56px xuống **42px**.
- Thu gọn cột **Địa bàn** từ 190px xuống **135px**.
- Cột Địa bàn vẫn cố định khi kéo ngang.
- Cho phép tên địa bàn dài xuống tối đa nhiều dòng trong cùng một ô để không bị mất chữ.
- Giảm padding để hiển thị thêm nhiều cột chỉ tiêu hơn trên cùng màn hình.

- Thu gọn thêm cột **XH** xuống **36px**.
- Thu gọn cột **Địa bàn** xuống **108px**.
- Giảm padding và cỡ chữ ở toàn bộ bảng 22 địa bàn.
- Thu gọn các cột chỉ tiêu để hiển thị thêm nhiều thông tin trên cùng màn hình.
- Giữ nguyên cơ chế cố định cột XH và Địa bàn khi kéo ngang.

- Thu gọn cột **Địa bàn** từ 108px xuống **95px**.
- Căn kích thước sát với tên dài như **Dương Minh Châu**.
- Giảm padding ngang còn 2px.
- Giữ nguyên cơ chế cố định cột khi kéo ngang.
- Tên quá dài sẽ hiển thị dấu `...` thay vì làm rộng bảng.

- Thu gọn cột **XH** xuống **30px**.
- Thu gọn cột **Địa bàn** xuống **78px**.
- Giảm khoảng cách giữa cột XH và Địa bàn.
- Giảm padding ngang trong toàn bộ bảng.
- Thu gọn thêm các cột chỉ tiêu để hiển thị được nhiều thông tin hơn.
- Vẫn giữ cố định cột XH và Địa bàn khi kéo ngang.

- Khóa cứng cột **XH** và **Địa bàn** bằng `position: sticky` với `z-index` ưu tiên cao.
- Cột Địa bàn luôn đứng yên khi kéo ngang.
- Header tiếp tục cố định khi cuộn dọc.
- Dòng tổng tiếp tục cố định ở cuối vùng bảng.
- Bổ sung `translateZ(0)` để tăng độ ổn định trên Chrome và trình duyệt di động.

- Điều chỉnh cơ chế cố định cột:
  - **Chỉ cột Địa bàn đứng im** khi kéo ngang.
  - Cột **XH di chuyển theo bảng**, không còn cố định bên trái.
- Cột Địa bàn được đặt tại `left: 0` để luôn sát mép trái vùng bảng.
- Header và dòng tổng vẫn cố định khi cuộn dọc.
