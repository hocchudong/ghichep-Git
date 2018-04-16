# Git là gì? Những lợi ích của việc dùng Git?
---
## Git là gì?
`Git` là tên gọi của một `Hệ thống quản lý phiên bản phân tán` (`Distributed Version Control System – DVCS`) là một trong những hệ thống quản lý phiên bản phân tán phổ biến nhất hiện nay.

`DVCS` giúp mỗi PC có thể `lưu trữ` nhiều `phiên bản khác nhau` của 1 bộ mã nguồn đã được nhân bản (`clone`) từ một kho chứa mã nguồn (`repository`), các thay đổi trên mã nguồn sẽ được `commit` rồi đưa lên server nơi đặt kho chứa chính. Các PC khác (có quyền truy cập) cũng có thể `clone` lại mã nguồn từ kho chứa để lấy phiên bản mới nhất. Trong Git, khái niệm này gọi là `Working Tree`.


`Git` ưu việt hơn các hệ thống quản lý code thông thường vì có `khả năng tách nhánh` (branch), hỗ trợ rất tốt cho teamwork, vì những việc như phân chia task, tổng hợp code trở nên dễ dàng hơn nhiều.

## Mô hình tổng quan

![](../images/git-overview-fb-1.png)

## Điểm giống và khác giữa git và các hệ thống quản lý code
### 1. Giống:
- Git là một hệ thống quản lý phiên bản (viết tắt: VCS), hỗ trợ:
 - Quản lý code và lịch sử thay đổi.
 VD: Cập nhật code, chỉnh sửa code nhanh hơn, theo dõi các thay đổi thuận tiện, dễ dàng quay lại phiên bản cũ nếu xuất hiện lỗi
 - Làm việc nhóm.
 VD: Làm việc nhóm trở nên đơn giản hơn khi sử dụng nhưng tính năng như `branch`

### 2. Khác:
- Git tiếp cận theo hướng `phân tán` (distributed approach)
- Điểm khác biệt lớn nhất là khả năng tách nhánh (branch).

 => Git hỗ trợ rất tốt cho teamwork, vì những việc như phân chia task, tổng hợp code trở nên dễ dàng hơn nhiều. (tìm hiểu them "git flow")

## Lợi ích của Git
- Sắp xếp công việc tốt hơn.
  Có thể tập trung giải quyết từng task mà không phải bận tâm lo lắng cho những task liên quan.
- Linh hoạt hơn khi phải làm cùng lúc nhiều task , bởi cấu trúc phân tán git.
- Tự tin hơn khi thử nghiệm những ý tưởng mới, vì có thể tách biệt việc thử nghiệm với dự án chính. Điều này giúp nâng cao chất lượng code cũng như tính sáng tạo.




 https://itviec.com/blog/git-la-gi/
