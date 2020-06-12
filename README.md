## a
...
# Học git
## I Tạo folder và kết nối
b1: Tạo một folder ở trong ổ đỉa mà bạn muốn lưu trữ dự án
b2: Vào folder đó ->view-> bật Hidden items
b3: Vào cmd ở trong folder đó
b4: Gõ "git status" //xem git hoạt động chưa
b5: "git remote add origin [link của dự án mình tạo trên github]" //origin là tên được đặt cho link
b6: "git remote -v" //xem có bị lỗi gì không

## II Thực hiện các chức năng
1. Đẩy dử liệu lên github
b1: "git add --all" //Thêm tất cả các file có trong folder lên git
b2: "git commit -m "[tên mà bạn muốn tạo cho commit đó khi đẩy lên github]"
b3: "git log" hoặc "gitk" //xem tạo commit thành công chưa
b4: "git push [ten của dự án "origin là tên mọi người đang dùng->nên đặt như vậy ở phần I bước 5"] master"
    // đẩy commit đó lên
2. "git restore [tên file được lưu ở máy tính]" //Đưa dữ liệu quay về file ban đầu khởi tạo chưa qua chỉnh sửa
3. Quay lại các bước thực hiện trước
b1: "gitk"
b2: chọn tên commit chứa phần muốn quay lại
b3: Copy id của commit ở SHA1 
b4: Sang cmd gõ "git reset --hard [địa chỉ id đã copy ở b3]
Lưu ý: khi muốn xóa commit gì nên copy id commit đó để lưu dữ lại phòng khi xóa xong lại muốn lấy lại
4. "git push origin master -f" //đẩy file README.md lên github
...