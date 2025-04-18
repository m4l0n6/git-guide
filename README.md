# 📦 Hướng dẫn Git cho Dự án

## ✅ Thiết lập ban đầu

1. **Fork** repo (nếu là repo của người khác)
2. **Clone** về máy:
```bash
git clone https://github.com/<username>/<tên-repo>.git
```

3. **Di chuyển vào thư mục dự án:**
```bash
cd <tên-repo>
```

4. **Thêm remote gốc (nếu cần):**
```bash
git remote add upstream https://github.com/<tên-team>/<tên-repo>.git
```

---

## 🔄 Cập nhật code mới nhất

```bash
git fetch origin
git checkout main
git pull origin main
```

Nếu có remote `upstream`:
```bash
git fetch upstream
git merge upstream/main
```

---

## 🌿 Tạo nhánh mới để làm việc

```bash
git checkout -b ten-nhanh-moi
```
Ví dụ:
```bash
git checkout -b feature/add-login
```

---

## 💾 Lưu và đẩy thay đổi

1. **Kiểm tra trạng thái:**
```bash
git status
```

2. **Thêm thay đổi:**
```bash
git add .
```

3. **Commit:**
```bash
git commit -m "Mô tả ngắn gọn thay đổi"
```

4. **Push lên GitHub:**
```bash
git push origin ten-nhanh-moi
```

---

## 🚀 Tạo Pull Request (PR)

- Vào GitHub, tạo PR từ nhánh bạn vừa push lên.
- Gắn label nếu có.
- Gửi cho người review hoặc chờ merge.

---

## ⚠️ Lưu ý khi làm việc nhóm

- Mỗi tính năng nên được làm trên 1 nhánh riêng.
- Tránh commit trực tiếp vào `main`.
- Luôn **pull code mới nhất** trước khi làm.
- Đặt tên nhánh rõ ràng: `feature/`, `fix/`, `hotfix/`, `refactor/`,...

---

## 🔁 Rebase (tuỳ chọn, nâng cao)

```bash
git checkout feature/ten-nhanh
git pull --rebase origin main
```