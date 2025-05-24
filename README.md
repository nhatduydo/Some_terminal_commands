## một số lệnh comment terminal  
# MỤC LỤC
1. [xem các danh sách các extension đã cài trong máy](#xem-các-danh-sách-các-extension-đã-cài-trong-máy)
2. [xuất danh sách các extension đã cài trong máy](#xuất-danh-sách-các-extension-đã-cài-trong-máy)
3. [kiểm tra version của git](#kiểm-tra-version-của-git)
4. [kiểm tra phiên bản python](#kiểm-tra-phiên-bản-python)
5. [kiểm tra phiên bản của pip](#kiểm-tra-phiên-bản-của-pip)
6. [tạo môi trường ảo](#tạo-môi-trường-ảo)
7. [Chạy môi trường ảo](#chạy-môi-trường-ảo)
8. [Hủy kích hoạt môi trường ảo](#hủy-kích-hoạt-môi-trường-ảo)
9. [Cài đặt gói thư viện](#cài-đặt-gói-thư-viện)
10. [ghi danh sách các package thư viện đã cài vào requirements.txt](#ghi-danh-sách-các-package-thư-viện-đã-cài-vào-requirements.txt)
11. [cài các thư viện từ requirements](#cài-các-thư-viện-từ-requirements)
12. [Tạo gitignore](#tạo-gitignore)
13. [đổi khoảng cách indent (khoảng thụt dòng)](#đổi-khoảng-cách-indent-khoảng-thụt-dòng)
14. [cách tạo venv](#cách-tạo-venv)
15. [nếu tạo venv ở ngoài](#nếu-tạo-venv-ở-ngoài)
16. [kiểm tra phiên bản python](#kiểm-tra-phiên-bản-python)
17. [thu gọn code trong vscode](#thu-gọn-code-trong-vscode)
18. [mở rộng code trong vscode](#mở-rộng-code-trong-vscode)
19. [Lỗi "Import 'streamlit' could not be resolved"](#lỗi-import-streamlit-could-not-be-resolved)
20. [Chọn đúng Interpreter](#chọn-đúng-interpreter)  
21. [các extensions hỗ trợ format code python](#các-extensions-hỗ-trợ-format-code-python)
22. [SSH](#ssh)
    - [kiểm tra phiên bản](#kiểm-tra-phiên-bản)
    - [tạo cặp khóa public và private](#tạo-cặp-khóa-public-và-private)
    - [chứng thực ssh](#chứng-thực-ssh)
    - [xóa tài khoản đang chạy](#xóa-tài-khoản-đang-chạy)
23. [một số lệnh git](#một-số-lệnh-git)
    - [kiểm tra trạng thái](#kiểm-tra-trạng-thái)
    - [kiểm tra nhánh](#kiểm-tra-nhánh)
    - [tạo nhánh mới](#tạo-nhánh-mới)
    - [chuyển nhánh](#chuyển-nhánh)
    - [tạo và đồng thời chuyển sang nhánh mới](#tạo-và-đồng-thời-chuyển-sang-nhánh-mới)
    - [so sánh sự khác biệt giữa bản cũ và mới](#so-sánh-sự-khác-biệt-giữa-bản-cũ-và-mới)
    - [tạo PR Pull request trộn nhánh](#tạo-pr-pull-request-trộn-nhánh)
    - [giải quyết xung đột](#giải-quyết-xung-đột)
24. [git stash - lưu những thay đổi tạm thời vào thùng chứa tạm](#git-stash---lưu-những-thay-đổi-tạm-thời-vào-thùng-chứa-tạm)
25. [đưa file về trạng thái cũ như ban đầu](#đưa-file-về-trạng-thái-cũ-như-ban-đầu)
26. [chuyển file từ vùng xanh staging area quay lại đỏ working copy](#chuyển-file-từ-vùng-xanh-staging-area-quay-lại-đỏ-working-copy)
27. [bỏ file khi đã lỡ push lên server](#bỏ-file-khi-đã-lỡ-push-lên-server)
28. [Hướng dẫn ubuntu song song](#Hướng-dẫn-ubuntu-song-song)














## xem các danh sách các extension đã cài trong máy
```
code --list-extensions
```
## xuất danh sách các extension đã cài trong máy
```
code --list-extensions > extensions-list.txt
```
## kiểm tra version của git
```
git --version 
```
## kiểm tra phiên bản python
```
python --version
```
## kiểm tra phiên bản của pip
```
pip --version
```
## tạo môi trường ảo
```
python -m venv .venv
```
## Chạy môi trường ảo
```
.\venv\Scripts\activate
```
## Hủy kích hoạt môi trường ảo
```
deactivate
```
## Cài đặt gói thư viện
```
pip install <name_package>
```
## ghi danh sách các package thư viện đã cài vào requirements.txt
```
pip freeze > requirements.txt
```
## cài các thư viện từ requirements
```
pip install -r requirements.txt
```
## Tạo gitignore
đến thư mục chứa dự án
```
echo.> .gitignore
```
## đổi khoảng cách indent (khoảng thụt dòng)
ctrl + shift + p => Change tab display size => chọn 4 (mặc định)

## cách tạo venv
tạo venv ngang cấp với folder chạy chương trình
vd:
- khachsan
+ .idea
+ app
+ venv

active như bình thường
```
.\venv\Scripts\activate
```
khi chạy file:
```
python -m app.index
```
```
python -m app.models
```

## nếu tạo venv ở ngoài
phải set PYTHONPATH
```
$env: PYTHONPATH = "D:\QLkhachSan\khachsan"
```
```
.venv\Scripts\python.exe khachsan\app\index.py
```
nếu không được thử set PYTHONPATH bằng cách này
```
set PYTHONPATH = D:\QLkhachSan\khachsan
```
```
.venv\Scripts\python.exe khachsan\app\index.py
```
## kiểm tra phiên bản python
```
py -0
```
## thu gọn code trong vscode
ctrl + shift + [
## mở rộng code trong vscode
ctrl + shift + ]
## format code html
ctrl + shift + f
## Lỗi "Import 'streamlit' could not be resolved"
thường xảy ra khi VS Code không thể tìm thấy thư viện streamlit trong môi trường Python hiện tại. Dưới đây là một số bước bạn có thể thử để khắc phục vấn đề này:
## Chọn đúng Interpreter
Nhấn Ctrl+Shift+P để mở Command Palette.
Gõ Python: ```Select Interpreter``` và chọn đúng phiên bản Python mà bạn đã cài đặt streamlit.
streamlit run chatbot.py
## các extensions hỗ trợ format code python
- black formatter
- pep8
- yapf
## SSH
## kiểm tra phiên bản
```
ssh -V
```
## tạo cặp khóa public và private
```
ssh-keygen
```
enter lấy mặc định
vào thường dẫn sẽ thấy 2 cặp khóa được tạo ra 
```
C:\Users\nhatduy\.ssh
```
gồm 2 loại: id_ed123 và id_ed123.pub
+ id_ed123 => khóa private key
+ id_ed123.pub => đây là khóa public key, khi vô công ty, nếu sếp yêu cầu đưa khóa cho ổng => đưa khóa public

## chứng thực ssh
- vào setting => SSH and GPG keys => new SSH => ghi title và paste ssh vô => oke
- kể từ thòi điểm chứng thực ssh => khi push lên là không cần chứng thực nữa
## xóa tài khoản đang chạy 
tìm kiếm: Credential Manager => Windows Credentials: chọn tài khoản github => remove
## một số lệnh git

```git clone```   
```git add```: working copy => staging area  
```git commit```: staging area =>  local repos  
```git push```: local repos => local repos  
## kiểm tra trạng thái
```
git status
```
## kiểm tra nhánh 
```
git branch
```
## tạo nhánh mới
```
git branch <tên_nhánh>
```
## chuyển nhánh
```
git checkout <tên_nhánh>
```
## tạo và đồng thời chuyển sang nhánh mới
```
git checkout -b <tên_nhánh>
```
nếu bạn đang sử dụng Git phiên bản mới hơn
```
git switch -c <tên_nhánh>
```
## so sánh sự khác biệt giữa bản cũ và mới
```
git diff
```
git diff (so sánh sự khác biệt) => nhấn q để thoát (quit)
git status => git add => git commit -m "" => git push tennhanh
## tạo PR Pull request trộn nhánh 
```
git pull 
```
## giải quyết xung đột
khi xảy ra xung đột, không giải quyết trên github, chỉ có thể giải quyết cục bộ 
dưới cục bộ chuyển từ nhánh chính main => nhánh con: vd duy
- git checkout duy (di chuyển qua nhánh duy)
- git merge main => máy sẽ báo xung đột mã     nguồn, vào code xem phần code bị xung đột mã nguồn => sửa code bị lỗi => test lại 
- sau khi sửa xong push lên lại 
- git status => git add .... => git commit -m "" => git push origin duy
- lúc này phần mearge đang vàng sẽ tự động chuyển xanh nếu hết lỗi
Ví dụ cụ thể:
 - nhánh duy: sửa file duy.txt và push lên nhánh duy
 - nhánh main: không biết, cũng sửa file duy.txt và push lên main
 - nhánh duy merge origin main => lỗi:
```
$ git merge origin
Auto-merging tri.txt
CONFLICT (content): Merge conflict in tri.txt
Automatic merge failed; fix conflicts and then commit the result.
```
Quy tắc: sửa lỗi trên nhánh của mình, chay test thử code => hết lỗi thì push lên lại nhánh duy
lúc này, merge sẽ tự động báo xanh 
=> thực hiện merge với nhánh main 
đã giải quyết xong
```
git status
```
```
git add duy.txt
```
```
git commit -m 'fix bug merge'
```
```
git push origin duy
```
```
 git merge origin main
```

## git stash - lưu những thay đổi tạm thời vào thùng chứa tạm
- lưu những thay đổi tạm thời vào thùng chứ tạm
  ```
  git stash
  ```
- xem danh dánh đã lưu
  ```
  git stash list
  ```
- áp dụng lại stash
- + apply hết
    ```
    git stash apply
    ```
  + apply 1 cái nào đó
    ```
    git stash list
    ```
    ```
    git stash apply {name}
    ```
    
## đưa file về trạng thái cũ như ban đầu
```
git checkout namefile
```
ví dụ: git checkout text.txt
chỉ có tác dụng ở vùng đỏ (trước git add) khi chuyển qua xanh (sau khi git add) thì không còn tác dụng
## chuyển file từ vùng xanh stagging area quay lại đỏ working copy
nếu file đã thực hiện git add mà muốn quay lại thì thực hiện 
```
git reset filename
```
còn nếu đã lỡ nằm trên thùng chứa cục bộ luôn thì chỉ có thể reset thùng chứa lại 
## bỏ file khi đã lỡ push lên server
khi đã lỡ thực hiện tất cả bước: 
git add => git commit => git push mà muốn gỡ file đã push trên server thực hiện
```
git rm filename
```
```
git commit -m ""
```
```
git push origin main
```
# Hướng dẫn ubuntu song song
Khởi động vào Ubuntu.
Mở file cấu hình GRUB:
```
sudo nano /etc/default/grub
```
```
GRUB_DEFAULT="Windows Boot Manager (on /dev/sda1)"
```
Tìm dòng: ```GRUB_DEFAULT=0```
và thay bằng: 
```
GRUB_DEFAULT="Windows Boot Manager (on /dev/sda1)"
```
