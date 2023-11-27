# Web bán sách

## Các module:

### `discovery-server`: để registry discovery service, chứa cấu hình và cài đặt cho Eureka Server

### `api-gateway`: để định tuyến các request đến các service khác

### `common`: chứa các class, interface, enum, ... dùng chung cho các module khác

### `user`: quản lý người dùng
- Register, forgot password
- Login: login basic authentication, login bằng oauth 2
- Profile: getProfile, changePassword, updateProfile
- CRUD, search user
- Role: admin, user, ownerShop

### `book`: quản lý sách
- Book Combo: bộ truyện tranh
- CRUD book, book combo
- Bán sách theo bản mềm và bản cứng
- Search theo tên, thể loại, tác giả, nhà xuất bản, giá, năm...

### `publisher`: quản lý nhà xuất bản
- CRUD, search publisher

### `author`: quản lý tác giả
- CRUD, search author

### `category`: quản lý thể loại
- CRUD, search category

### `cart`: quản lý giỏ hàng
- CRUD, search cart
- Thanh toán bằng thẻ và tiền mặt đối với sách bản cứng, bản mềm chuyển khoản thành công sẽ tự động share sách qua drive cho khách hàng

### `bill`: quản lý hóa đơn
- CRUD, search bill

### `review`: quản lý đánh giá
- CRUD, search review theo sách

### `notification`: quản lý thông báo