Deploy sản phẩm
- chạy npm install để cài đặt dependency
- chạy npx hardhat compile để compile hardhat
- chạy npx hardhat node để khởi động hardhat, lưu lại 20 tài khoản được hardhat emulate
- chạy npx hardhat run scripts/deploy.js --network localhost để deploy tài khoản nhận thanh toán hardhat, lưu lại địa chỉ deploy và thay vào contractaddress trong file app.js
- di chuyển tới folder frontend
- chạy npm install để cài đặt dependency
- chạy npm start

Cấu hình và link sản phẩm tới Metamask
- Lựa chọn mục network
- Chọn add network manually và thêm mạng localhost với RPC URL là http://localhost:8545 do Hardhat node được host mặc định tại port 8545
- Lựa chọn thêm Account, thêm account bằng private key được tạo bởi hardhat node
- Connect tài khoản vừa tạo tới localhost

Sử dụng sản phẩm
- Sản phầm bao gồm 3 phần chính : Upload image (ví dụ thay thế cho nft), get data và share
Upload image:
- Lựa chọn add ảnh vào tài khoản, khi add ảnh metamask sẽ pop up yêu cầu confirm transaction
- Xác nhận transaction để upload image
Get data:
- Nhập private key vào ô trống và chọn get data
- NFT dc hiển thị nếu như account với private key nói trên có quyền truy cập
Share:
- Di chuyển tới tài khoản đã upload file ảnh nft bằng cách thay đổi tài khoản trên Metamask
- Chọn mục share, nhập key và confirm transaction

  
