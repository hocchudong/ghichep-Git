# Thao tác nâng cao trên Remote Repo và Origin
---
## Vấn đề
Remote Repo ta sử dụng ở đây là Github. Nó là một máy chủ repository - (Remote Repository), tức repository chính sẽ không nằm trên máy tính của cá nhân.

Thông thường để Update dữ liệu lên, ta sử dụng:
```
git push origin master
```

> Mặc định khi clone một repository thì nó tự đặt tên là origin

__Kiếm tra remote__
```shell
lacoski@lacoski-PC:~/GitRepo/tim-hieu-git$ git remote -v

origin	https://github.com/lacoski/tim-hieu-git.git (fetch)
origin	https://github.com/lacoski/tim-hieu-git.git (push)
```

Các repository sẽ đều có hai hành động:
- fetch (lấy dữ liệu về từ server)
- push (gửi dữ liệu lên server)

## Đổi tên remote
Ta có thể đổi tên `origin` bằng 1 tên khác cho việc quản lý trong trường hợp có nhiều Remote trong 1 dự án:

__Cú pháp__
```shell
git remote rename [tên_cũ] [tên_mới]
```

VD:
```
lacoski@lacoski-PC:~/GitRepo/tim-hieu-git$ git remote rename origin lacoski
lacoski@lacoski-PC:~/GitRepo/tim-hieu-git$ git remote -v

lacoski	https://github.com/lacoski/tim-hieu-git.git (fetch)
lacoski	https://github.com/lacoski/tim-hieu-git.git (push)
```

## Thêm 1 remote
__Cú pháp__
```
git remote add [tên_remote] URL
```
VD:
```shell
lacoski@lacoski-PC:~/GitRepo/tim-hieu-git$ git remote add test https://github.com/lacoski/tim-hieu-git.git
lacoski@lacoski-PC:~/GitRepo/tim-hieu-git$ git remote -v

origin	https://github.com/lacoski/tim-hieu-git.git (fetch)
origin	https://github.com/lacoski/tim-hieu-git.git (push)
test https://github.com/lacoski/tim-hieu-git-1.git (fetch)
test https://github.com/lacoski/tim-hieu-git-1.git (push)
```

__Lấy dữ liệu từ Repo mới__
```
git fetch [tên remote]
```
> Lệnh đơn thuần update database repo chứ không gộp vào Repo đang làm việc.

Gộp dữ liệu trên Repo
```
git merge [tên remote]/[nhánh]
```

## Sự khác nhau giữa clone, fetch và pull
3 lệnh để lấy dữ liệu về từ repository nhưng có sự khác nhau:

__git clone__

Sao chép toàn bộ dữ liệu trên repository và sao chép luôn các thiết lập về repository, tức là nó sẽ tự động tạo một master branch trên máy tính.

> Lệnh này chỉ nên sử dụng khi cần tạo mới Git repo trên máy tính với toàn bộ dữ liệu và thiết lập của một remote repository.

__git pull__

Tự động lấy toàn bộ dữ liệu từ remote repository và gộp vào cái branch hiện tại đang làm việc.

__git fetch__

Lấy toàn bộ dữ liệu từ remote repository nhưng sẽ cho phép gộp thủ công vào một branch nào đó trên thư mục Git ở máy tính.

> Về Branch xem thêm tại các docs sau

## Nguồn

https://thachpham.com/tools/git-so-luoc-remote-respository-va-origin.html
