# Tạo repository (repo)
## git init
## =>Nhánh chính : master

### git init -b main
### =>Tạo repo local vs nhánh chính tên main

### git branch -M main
### Đổi tên

## git remote add origin + <url repo>
## =>Liên kết repo local với repo remote

# Không đưa thư mực node_modules lên repo remote
# => Node_modules chiếm dung lượng rất lớn
# => Node_modules có thể cài lại thông qua câu lệnh : npm i

# File .gitignore quy định những thư mục hay file không được phép đẩy lên repo remote 
# => .gitignore nằm ở thư mục root

# git status
# => Kiểm tra sự thay đổi của các file trong dự án

# git add . => Dùng để thêm tất cả file ở trong thư mục hiện tại vào trong staging

# git add -A => Dùng để thêm tất cả các file ở trong dự án vào trong staging

# git add => <đường dẫn file> => Chỉ thêm file cụ thể vào trong staging
