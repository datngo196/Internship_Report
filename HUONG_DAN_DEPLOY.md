# Hướng dẫn Deploy Hugo Site lên GitHub Pages

## Bước 1: Kiểm tra và cập nhật cấu hình

### 1.1. Kiểm tra baseURL trong config.toml
- Mở file `config.toml`
- Kiểm tra dòng `baseURL` - nó phải khớp với URL GitHub Pages của bạn
- Format: `https://[username].github.io/[repository-name]/`
- Ví dụ: Nếu repository của bạn là `my-username/my-repo`, thì baseURL sẽ là `https://my-username.github.io/my-repo/`

## Bước 2: Thêm file workflow vào git

```bash
git add .github/workflows/gh-pages.yml
git commit -m "Add GitHub Actions workflow for GitHub Pages deployment"
```

## Bước 3: Tạo repository trên GitHub (nếu chưa có)

1. Đăng nhập vào GitHub: https://github.com
2. Click vào dấu **+** ở góc trên bên phải → chọn **New repository**
3. Đặt tên repository (ví dụ: `fcj-workshop-template`)
4. Chọn **Public** (GitHub Pages miễn phí cho public repo)
5. **KHÔNG** tích vào "Initialize with README" (vì bạn đã có code sẵn)
6. Click **Create repository**

## Bước 4: Kết nối local repository với GitHub

Nếu repository đã tồn tại trên GitHub và bạn đã có remote:
```bash
git remote -v
```

Nếu chưa có remote hoặc muốn thay đổi:
```bash
git remote add origin https://github.com/[username]/[repository-name].git
```

Hoặc nếu muốn thay đổi remote hiện tại:
```bash
git remote set-url origin https://github.com/[username]/[repository-name].git
```

## Bước 5: Push code lên GitHub

```bash
git add .
git commit -m "Prepare for GitHub Pages deployment"
git push -u origin master
```

**Lưu ý:** Nếu repository của bạn dùng branch `main` thay vì `master`:
```bash
git push -u origin master:main
```

## Bước 6: Bật GitHub Pages

1. Vào repository trên GitHub
2. Click vào tab **Settings** (ở menu trên cùng)
3. Scroll xuống phần **Pages** (ở sidebar bên trái)
4. Trong phần **Source**, chọn:
   - **Source**: `GitHub Actions`
5. GitHub sẽ tự động phát hiện workflow file và bắt đầu build

## Bước 7: Kiểm tra quá trình deploy

1. Vào tab **Actions** trong repository
2. Bạn sẽ thấy workflow "Deploy Hugo site to GitHub Pages" đang chạy
3. Click vào workflow để xem chi tiết
4. Đợi khoảng 2-5 phút để build hoàn tất
5. Khi thành công, bạn sẽ thấy dấu tích màu xanh

## Bước 8: Truy cập website

Sau khi deploy thành công:
- URL sẽ là: `https://[username].github.io/[repository-name]/`
- GitHub sẽ hiển thị URL trong tab **Settings → Pages**

## Troubleshooting

### Lỗi: Workflow không chạy
- Kiểm tra xem file `.github/workflows/gh-pages.yml` đã được commit chưa
- Đảm bảo bạn đã push lên branch `main` hoặc `master`

### Lỗi: Build failed
- Kiểm tra tab **Actions** để xem log chi tiết
- Đảm bảo Hugo theme đã được cài đặt đúng (submodule)

### Lỗi: 404 Not Found
- Kiểm tra baseURL trong `config.toml` có đúng không
- Đảm bảo repository là **Public**
- Đợi vài phút để GitHub cập nhật DNS

### Cập nhật website sau khi thay đổi code
Chỉ cần push code mới lên GitHub:
```bash
git add .
git commit -m "Update content"
git push
```
GitHub Actions sẽ tự động build và deploy lại!

