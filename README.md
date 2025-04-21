# 📘 CÁC BƯỚC LÀM VIỆC NHÓM TRÊN GITHUB

## 1. 🧭 Sao chép Repository (Clone)
Mỗi thành viên clone repository về máy của bản thân:
```bash
git clone <URL_repo>
```

## 2. 🌿 Tạo Nhánh (Branch)
Mỗi thành viên tạo một nhánh mới từ nhánh `main` để thực hiện công việc của bản thân:
```bash
git checkout -b <ten_nhanh>
```

## 3. 💻 Thực hiện công việc
Các thành viên thực hiện thay đổi, sau khi hoàn tất kiểm tra, sử dụng các lệnh:
```bash
git add .
git commit -m "<thay_doi>"
```

## 4. 🔄 Đồng bộ Nhánh Main
Trước khi push, đảm bảo rằng nhóm đã cập nhật nhánh `main` từ remote:
```bash
git checkout main
git pull origin main
```

Sau đó quay lại nhánh của bạn và rebase nếu cần:
```bash
git checkout <ten_nhanh>
git rebase main
```

## 5. ⬆️ Push Nhánh Lên GitHub
```bash
git push origin <ten_nhanh>
```

## 6. 🚀 Tạo Pull Request (PR)
- **Tạo PR:** Vào GitHub, chọn nhánh của bạn vừa push lên và nhấn “Compare & pull request”.
- **Tiêu đề rõ ràng:** Đặt tiêu đề và mô tả ngắn gọn nội dung thay đổi.
- **Reviewer:** Gán người review nếu cần.
- **Thảo luận:** Thành viên khác có thể bình luận góp ý code.
- **Merge:** Sau khi được duyệt, nhóm trưởng hoặc người có quyền sẽ merge vào `main`.

## 7. 🔀 Merge PR hoặc Merge thủ công
Nếu không dùng GitHub, có thể merge thủ công bằng dòng lệnh:
```bash
git checkout main
git merge <feature_branch>
git push origin main
```

## 8. 🔃 Cập Nhật và Pull
Các thành viên khác cần cập nhật repository local của họ sau khi merge:
```bash
git checkout main
git pull origin main
```
