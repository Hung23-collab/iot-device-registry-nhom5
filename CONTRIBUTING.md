# Quy tắc đóng góp - Nhóm 5

Tài liệu này quy định quy trình làm việc và đóng góp mã nguồn cho dự án quản lý danh mục thiết bị IoT phòng lab (IoT Device Registry). Tất cả thành viên bắt buộc phải tuân thủ các quy tắc cốt lõi sau đây:

## 1. Quy tắc nhánh (Branching Policy)
* Tuyệt đối **không làm việc trực tiếp trên nhánh `main`**[cite: 1].
* Mỗi thành viên khi thực hiện nhiệm vụ phải tạo một nhánh riêng từ `main` mới nhất[cite: 1].
* Tên nhánh phải đặt tuân thủ cấu trúc: `feature/<mssv>-<noi-dung-ngan>`[cite: 1].
  * *Ví dụ:* `feature/20231234-data-model`[cite: 1].

## 2. Quy chuẩn thông điệp Commit (Commit Message Format)
Mỗi lần lưu lại thay đổi (commit), thông điệp phải viết theo mẫu: `<loai>: <mo-ta-ngan>`[cite: 1]. Các loại commit hợp lệ bao gồm[cite: 1]:
* `feat`: Khi thêm chức năng mới (mã nguồn ví dụ)[cite: 1].
* `docs`: Khi cập nhật hoặc thêm mới tài liệu (Markdown)[cite: 1].
* `test`: Khi viết thêm các ca kiểm thử (assert)[cite: 1].
* `chore`: Các thay đổi nhỏ về cấu hình hệ thống, `.gitignore`[cite: 1].

## 3. Quy trình Pull Request (PR) và Xem xét mã nguồn (Review)
1. Sau khi hoàn thành phần việc và đẩy nhánh lên GitHub, thành viên tiến hành tạo Pull Request (PR) hướng về nhánh `main`[cite: 1].
2. **Người tạo PR không được tự ý merge PR của chính mình**[cite: 1].
3. PR phải được ít nhất một thành viên khác trong nhóm xem xét (Review), để lại nhận xét (`--comment-body`) hoặc phê duyệt (`--approve`) trước khi hòa trộn[cite: 1].
4. Nếu nhận được yêu cầu sửa đổi (`--request-changes`), tác giả phải cập nhật lại mã nguồn trên chính nhánh đó cho đến khi được Approve[cite: 1].

## 4. Sau khi Hòa trộn (Post-Merge)
Khi PR đã được Maintainer hòa trộn vào nhánh `master` thành công, tất cả thành viên phải cập nhật lại mã nguồn local bằng cách chuyển sang nhánh `master` và chạy lệnh `git pull origin master` trước khi bắt đầu phần việc tiếp theo[cite: 1].