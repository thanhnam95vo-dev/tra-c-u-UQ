# Chương trình đồng hành cùng Điểm ủy quyền

## 1. Giới thiệu

Đây là phiên bản website dành cho **Điểm ủy quyền (ĐUQ)** tra cứu thông
tin bán hàng và theo dõi chương trình tri ân.

File HTML hiện tại:

`index_diem_uy_quyen_cap_nhat_den_19-08-2026.html`

Phiên bản dành cho ĐUQ đã được tinh gọn, không hiển thị các chức năng
quản trị nội bộ như **Tổng quan** và **Theo dõi 22 địa bàn**.

## 2. Chức năng hiện có

Website gồm 2 chức năng chính:

### Tri ân 18/08/2026

Phần Tri ân chỉ sử dụng dữ liệu bán hàng **riêng ngày 18/08/2026**,
không cộng dồn với các ngày khác.

Thể lệ giải thưởng:

  Giải              Số lượng tối đa      Mức thưởng   Điều kiện doanh thu
  --------------- ----------------- --------------- ---------------------
  Giải đặc biệt                   1        500.000đ         Từ 3.000.000đ
  Giải nhất                       1        300.000đ         Từ 2.000.000đ
  Giải nhì                        3   200.000đ/giải         Từ 1.000.000đ
  Giải ba                         5   100.000đ/giải           Từ 500.000đ

Dữ liệu cập nhật mới nhất cho ngày 18/08/2026:

-   **87 thuê bao PTM**
-   **13.612.000đ doanh thu**
-   **6 Điểm ủy quyền đủ điều kiện nhận giải**

Việc xét giải được thực hiện theo mức doanh thu và số lượng giải tối đa
của từng hạng.

### Tra cứu Điểm ủy quyền

Phần Tra cứu sử dụng dữ liệu cộng dồn từ **01/08/2026 đến 19/08/2026**
theo file Excel cập nhật mới nhất.

Số liệu hiện tại:

-   **266 Điểm ủy quyền**
-   **1.111 thuê bao PTM**
-   **623 thuê bao PTM từ 70k**
-   **114.629.000đ doanh thu**
-   **210 Điểm ủy quyền có phát sinh PTM**

Người dùng có thể tìm kiếm ĐUQ và mở chi tiết để xem:

-   Tên Điểm ủy quyền
-   Địa bàn
-   Nhân viên hỗ trợ
-   Tổng thuê bao PTM
-   Thuê bao PTM từ 70k
-   Doanh thu
-   Danh sách thuê bao đăng ký thành công
-   Ngày và giờ đăng ký thành công của từng thuê bao
-   Doanh thu tương ứng của từng thuê bao

Danh sách chi tiết được sắp xếp theo thời gian đăng ký thành công mới
nhất.

## 3. Phạm vi dữ liệu

Nguồn dữ liệu hiện tại:

`Chương trình đồng hành cùng Điểm ủy quyền(7).xlsx`

Các sheet sử dụng là các sheet **đang hiển thị**, đặc biệt:

-   `TH`: danh mục và thông tin Điểm ủy quyền.
-   `Đơn hàng`: dữ liệu thuê bao, trạng thái đăng ký, thời gian thành
    công và doanh thu.

Phạm vi tính toán:

-   **Tri ân:** chỉ ngày 18/08/2026.
-   **Tra cứu:** từ 01/08/2026 đến 19/08/2026.
-   Dữ liệu đơn hàng mới nhất trong file Excel có thời gian thành công
    đến **19/08/2026 07:59:52**.

## 4. Cách sử dụng

Website là một file HTML độc lập. Có thể mở trực tiếp bằng trình duyệt
hoặc chạy bằng Live Server.

Ví dụ với Visual Studio Code:

1.  Đặt file HTML vào thư mục dự án.
2.  Mở thư mục bằng Visual Studio Code.
3.  Chạy file bằng **Live Server**.
4.  Truy cập trang trên trình duyệt.
5.  Sử dụng **Tri ân 18/8** hoặc **Tra cứu ĐUQ**.

Không cần cài đặt cơ sở dữ liệu hay máy chủ backend cho phiên bản hiện
tại.

## 5. Nguyên tắc khi cập nhật dữ liệu mới

Khi có file Excel mới:

1.  Chỉ đọc các sheet dữ liệu đang hiển thị.
2.  Đối chiếu ĐUQ bằng mã định danh trong dữ liệu, không suy đoán theo
    tên gần giống.
3.  Cập nhật dữ liệu Tra cứu từ ngày 01/08/2026 đến ngày mới nhất có
    trong file.
4.  Không làm thay đổi phạm vi của chương trình Tri ân 18/08/2026 nếu
    không có yêu cầu mới.
5.  Kiểm tra lại tổng PTM, PTM từ 70k, doanh thu và số ĐUQ có phát sinh.
6.  Kiểm tra chi tiết một số ĐUQ để bảo đảm số thuê bao, ngày đăng ký và
    doanh thu khớp với sheet `Đơn hàng`.

## 6. Lưu ý

Các số liệu trong website phụ thuộc vào file Excel nguồn tại thời điểm
cập nhật. Khi Excel có dữ liệu mới, file HTML không tự đồng bộ mà cần
được tạo/cập nhật lại từ nguồn mới.

Phiên bản README này tương ứng với dữ liệu cập nhật ngày **19/08/2026**.
