# Config git
git config --global user.name "Hung Nguyen"
git cogit config --global user.email "nguyenlehung007@gmail.com"

# Khởi tạo repository ở local (máy tính)
git init -b main

# Kiểm tra thay đổi code
git status

# Đưa code thay đổi vào stae để chuẩn bị đưa lên repo
git add <tên file>

git add . (đưa toàn bộ file đang thay đổi vào stae change, ngoại trừ file vừa xóa vào stage change)

git add -A (đưa tất cả file đã thay đổi vào stage change)

# add commit
git commit -m "nội dung commit" 
## Lưu ý: chạy git add trước khi commit

# Connect local repo với remote repo
git remote add origin <link git repo>

# push code từ local repo lên remote repo
git push -u origin main (chỉ cần gõ đầy đủ ở lần push đầu tiên) 
## chạy lệnh git commit trước khi git push
lần sau chỉ cần gõ git push

# git reset đưa file đang ở khu vực staged change về lại khu vực changes
git reset . => đưa toàn bộ file đang ở staged changed =>change
git reset <tên file> => chỉ đưa file ở staged changed =>change

<<<<<<< HEAD
# branch
git branch <tên branch> => tạo 1 branch mới

git switch <tên branch> => chuyển qua branch <tên branch>

git check out -b <tên branch> => tạo 1 branch mới và nhảy qua branch đó

git branch -m <tên branch mới> => đổi tên branch

=======
# git checkout <tên file> => đưa file về trang thái ban đầu

# Xem lịch sử commit:
git log
git log --oneline
=> để exit: nhấn phím Q

# branch
git branch => liệt kê branch đang có
git branch <tên branch> => tạo 1 branch mới
git switch <tên branch> => chuyển qua branch <tên branch>
git checkout -b <tên branch> => tạo 1 branch mới và nhảy qua branch đó
git branch -m <tên branch mới> => đổi tên branch
>>>>>>> feature/Login
git branch -D <tên branch> => xóa branch
=> đứng ở branch khác mới có thể xóa đc