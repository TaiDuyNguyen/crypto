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

# working directory (file màu đỏ) không thể đưa lên repo
# staging (file màu xanh lá) 
# => Lúc này file sẵn sàng để đưa lên repo

# congif git
### git config --global user.name "name"
### git config --global user.email "abc@email'

# git commit -m "mesage"
# => Dùng để gắn message vào trong những  file đang ở staging được phép đưa lên repo remote
# Mỗi commit có một cái mã sha(id)


# git log 
# => Dùng để kiểm tra lịch sử commit

# git push -u origin <tên nhánh>
# =>đưa code lên repo remote
# => từ lần push code thứ 2: git push
<<<<<<< HEAD
# Dis
=======

# Đưa file từ staging về lại woking
# git reset
# git restore -S . (Đưa tát cả các file đang ở staging về working)
# git restore -S<url flie> (Chỉ đưa duy nhát file về working)


# git checkout <url file>
# => 1. Đưa 1 file đang được chỉnh về trạng thái đó
# git checkout -b <tên nhánh>
=> tương đương với 2 lệnh git branch + git switch
# git checkout <tên nhánh>
=> tương đương với lệnh git switch
=> dùng để chuyển qua <tên nhánh>

### branch
/ Dev => kiểm thử QA và dev (dev)
// staging => QA kiểm thử 1 lần (staging)
/// production => end user (main/release)
# git branch <tên nhánh> 
Tạo ra 1 nhánh mới 
Nhánh mới sẽ chứa toàn bộ code của nhánh đang đứng

# git branch -a
=> Liệt kê tất các branch đang có trong repo

# git switch <tên nhánh>
=>Chuyển quan nhánh<Tên nhánh>
<!-- Đưa code từ github về máy -->
# git pull
=> Pull code ở repo remote về local

# git pull --no-ff (Nếu git pull bị lỗi thì thử lại)

### git clone <url repo>
=> Dùng  để clone soure code của 1 repo bất kì
<<<<<<< HEAD

# git meger <branch>
merge<branch> vào branch hiện tại
TH1 : merge thành công nếu không có bất kì sung đột (conflict)
TH2 : bị xung đột => giải quyết conflict => commit
=>Nếu merge code mà bị conflict => có thể hủy git merge thông qua lệnh : git merge --abort
=======
>>>>>>> main
>>>>>>> 0c128e90c2a2ee18e2aeebaa60678c5dc4fd58d7
