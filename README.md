Tất cả các cuộc thảo luận không liên quan trực tiếp đến mã trong yêu cầu kéo
  sẽ xảy ra trên [ bug.python.org ] (https://bugs.python.org/)
- Theo yêu cầu kéo không tầm thường đầu tiên của bạn (bao gồm các (cd);;( về tài liệu),
  vui lòng thêm chính bạn vào [ `Misc / ACKS` ] (https://github.com/python/cpython/blob/ master / Misc / ACKS)
  vui lòng thêm chính bạn vào [ `Misc / ACKS` ] (https://github.com/python/cpython/blob/ main / Misc / ACKS)


##  Đặt kỳ vọng
  2  buildbots.rst 
@@ -40,7 +40,7 @@ Có ba cách để hình dung kết quả xây dựng gần đây:
  https://code.google.com/archive/p/bbreport. Việc cài đặt nó rất đơn giản: chỉ cần thêm
  thư mục chứa `` bbreport.py '' đến đường dẫn hệ thống của bạn để
  bạn có thể chạy nó từ bất kỳ vị trí hệ thống tập tin nào. Ví dụ, nếu bạn muốn
  để hiển thị kết quả xây dựng mới nhất trên nhánh phát triển (" chính "),
  để hiển thị kết quả xây dựng mới nhất trên nhánh phát triển (" chính "),
  kiểu::

      bbreport.py -q 3.x
  12  cam kết. đầu tiên 
@@ -19,7 +19,7 @@ để vào cây nguồn chung. Hãy tự hỏi mình những câu hỏi sau đây:
   chúng ta cần phải có một giải pháp ở đó trước khi chúng ta có thể hợp nhất yêu cầu kéo.

* ** Yêu cầu kéo có được thực hiện đầu tiên đối với nhánh thích hợp không? ** 
   Nhánh duy nhất nhận được các tính năng mới là `` master '' , 
   Chi nhánh duy nhất nhận được các tính năng mới là `` chính '' ,
   chi nhánh đang phát triển. Yêu cầu kéo chỉ nên nhắm mục tiêu đến các nhánh sửa lỗi
   nếu sự cố chỉ xuất hiện trong phiên bản đó và có thể là các phiên bản cũ hơn.

@@ -161,15 +161,15 @@ Kho lưu trữ Python, vì vậy bạn cần phải cẩn thận với quy trình làm việc của mình:
  Bạn cũng có thể đẩy các nhánh này vào một kho lưu trữ công cộng riêng biệt
  cho công việc bảo trì trước khi nó được tích hợp vào kho lưu trữ chính.

* ** Bạn không nên tham gia trực tiếp vào nhánh **  `` master ''  ** hoặc bất kỳ nhánh nào trong số các nhánh bảo trì. **
* ** Bạn không nên tham gia trực tiếp vào nhánh **  `` chính ``  ** hoặc bất kỳ nhánh bảo trì nào. **
  Bạn nên cam kết với nhánh tính năng của riêng mình, sau đó tạo 
  yêu cầu kéo.

* ** Đối với một thay đổi nhỏ, bạn có thể thực hiện chỉnh sửa nhanh thông qua giao diện người dùng web GitHub. **
  Nếu bạn chọn sử dụng giao diện người dùng web, hãy lưu ý rằng GitHub sẽ
  tạo một nhánh mới trong kho CPython chính thay vì trong nhánh rẽ của bạn.
  Xóa nhánh mới tạo này sau khi nó đã được hợp nhất vào
  nhánh `` master '' hoặc bất kỳ nhánh bảo trì nào. Để duy trì CPython
  chi nhánh `` chính '' hoặc bất kỳ chi nhánh bảo trì nào. Để duy trì CPython
  kho lưu trữ gọn gàng, loại bỏ chi nhánh mới trong vòng vài ngày.

Giữ một nhánh của kho lưu trữ chính, vì nó sẽ cho phép bạn hoàn nguyên tất cả
@@ -187,7 +187,7 @@ Thấy các chi nhánh đang hoạt động

Nếu bạn sử dụng `` git branch '' , thì bạn sẽ thấy danh sách các nhánh : ref : `
<branchstatus> `. Chi nhánh duy nhất nhận được các tính năng mới là
`` master '' , nhánh đang phát triển. Các chi nhánh khác chỉ nhận
`` main '' , nhánh đang phát triển. Các chi nhánh khác chỉ nhận
sửa lỗi hoặc sửa chữa bảo mật.


@@ -207,15 +207,15 @@ tự backporting nó, sử dụng backport được tạo bởi cherry_picker.py_
như một điểm khởi đầu.

Bạn có thể lấy băm cam kết từ yêu cầu kéo ban đầu hoặc bạn có thể sử dụng
`` git log '' trên nhánh `` master '' . Để hiển thị 10 cam kết gần đây nhất
`` git log '' trên nhánh `` chính '' . Để hiển thị 10 cam kết gần đây nhất
băm và dòng đầu tiên của cam kết, sử dụng lệnh sau ::

   git log -10 --oneline

.. _ backport-pr-title :

Bạn có thể đặt tiền tố cho yêu cầu backport pull với nhánh và tham chiếu
số yêu cầu kéo từ `` master '' . Đây là một ví dụ::
số yêu cầu kéo từ `` chính '' . Đây là một ví dụ::

   [3.9] bpo-12345: Khắc phục mô-đun thư rác (GH-NNNN)

  2  coverity.rst 
@@ -150,4 +150,4 @@ Dakshesh Vyas <scan-admin@coverity.com>

.. _ Coverity Connect : https://scan.coverity.com/projects/py
-----------------

Các '' thầy '' chi nhánh là chi nhánh cho tính năng phiên bản tiếp theo; nó là
Các '' chính '' chi nhánh là chi nhánh cho tính năng phiên bản tiếp theo; nó là
đang được phát triển tích cực cho tất cả các loại thay đổi: tính năng mới, ngữ nghĩa
thay đổi, cải tiến hiệu suất, sửa lỗi.

@@ -57,7 +57,7 @@ đã cắt bản phát hành (ví dụ: phiên bản cuối cùng của 3.4.0).

Bắt đầu với bản phát hành 3.5, chúng tôi tạo nhánh bảo trì bản phát hành
(ví dụ: 3.5) tại thời điểm chúng tôi nhập phiên bản phép
phát triển tính năng cho bản phát hành 3.n + 1 xảy ra trong bản chính
phát triển tính năng cho bản phát hành 3.n + 1 xảy ra trong chính
phân nhánh cùng với phiên bản beta và phát hành các giai đoạn ổn định ứng viên
cho bản phát hành 3.n.

  59  gitbootcamp.rst 
@@ -103,17 +103,17 @@ Tạo và chuyển đổi chi nhánh
-------------------------------

.. quan trọng ::
   Không bao giờ cam kết trực tiếp với nhánh `` chính '' .
   Không bao giờ cam kết t
Điều này tương đương với ::

   # tạo một nhá
   git branch <branch-name> main
   # kiểm tra chi nhánh
   git checkout <branch-name>

@@ -144,7 +144,7 @@ Xóa nhánh

Để xóa một nhánh ** cục bộ ** mà bạn không cần nữa ::

   git tổng thể thanh toán
   git thanh toán chính
   git branch -D <branch-name>

Để xóa một nhánh ** từ xa ** ::
@@ -153,6 +153,19 @@ Để xóa một nhánh ** từ xa ** ::

Bạn có thể chỉ định nhiều nhánh để xóa.


Đổi tên chi nhánh
---------------

Nhánh mặc định của kho lưu trữ CPython đã được đổi tên từ `` chính '' thành `` chính ''
sau khi phát hành Python 3.10b1. Nếu bạn đã nhân bản kho lưu trữ trước đó
thay đổi, bạn có thể đổi tên chi nhánh cục bộ của mình như sau ::

    git branch -m master main
    git tìm nạp ngược dòng
    git nhánh -u ngược dòng / chính chính


Tệp dự trữ và cam kết
----------------------------

@@ -230,7 +243,7 @@ Tạo yêu cầu kéo

3. Nhấp vào liên kết `` so sánh giữa các ngã ba '' .

4. Chọn kho lưu trữ cơ sở: `` python / cpython '' và chi nhánh cơ sở: `` chủ '' .
4. Chọn kho lưu trữ cơ sở: `` python / cpython '' và chi nhánh cơ sở: `` chính

5. Chọn kho lưu trữ đầu: `` <tên người dùng> / cpython '' và phân nhánh đầu: chi nhánh
   chứa các thay đổi của bạn.
@@ -250,14 +263,14 @@ Tình huống:
  kho lưu trữ CPython ngược dòng.

Vui lòng không cố gắng giải quyết vấn đề này bằng cách tạo một yêu cầu kéo từ
`` python: master '' thành `` <username>: master '' như tác giả của các bản 
