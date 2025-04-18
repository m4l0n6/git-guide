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

## 5. 🔀 Merge Nhánh Của Mình vào Main
Merge nhánh của bạn vào nhánh `main`. Có thể thực hiện bằng GitHub hoặc dòng lệnh:
```bash
git checkout main
git merge <feature_branch>
```

## 6. 🚀 Tạo Pull Request (PR)
- **Tạo PR:** Thành viên tạo một Pull Request trên GitHub để đề xuất việc merge nhánh `feature_branch` vào `main`.
- **Kiểm tra và thảo luận:** Thành viên khác có thể kiểm tra và thảo luận về code trước khi merge.

## 7. ⬆️ Push Lên Repository
Sau khi merge, quản lý sẽ push nhánh `main` lên repository:
```bash
git push origin main
```

## 8. 🔃 Cập Nhật và Pull
Các thành viên khác cần cập nhật repository local của họ:
```bash
git pull origin main
```
