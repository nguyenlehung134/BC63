# Config git
git config --global user.name "Hung Nguyen"
git cogit config --global user.email "nguyenlehung007@gmail.com"

# Khởi tạo repository ở local (máy tính)
git init -b main

# Kiểm tra thay đổi code
git status

# Đưa code thay đổi vào stae để chuẩn bị đưa lên repo
git add <tên file>

git add . (đưa toàn bộ file đang thay đổi vào stae change)

git add -A (đưa những file đc thay đổi, ngoại trừ vừa tạo mới vào stae change)

# add commit
git commit -m "nội dung commit"

# Connect local repo với remote repo
git remote add origin <link git repo>

# push code từ local repo lên remote repo
git push -u origin main