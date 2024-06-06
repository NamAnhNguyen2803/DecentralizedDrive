Deploy sản phẩm
- chạy npm install để cài đặt dependency
- chạy npx hardhat compile để compile hardhat
- chạy npx hardhat node để khởi động hardhat, lưu lại 20 tài khoản được hardhat emulate
- chạy npx hardhat scripts/deploy.js --network localhost để deploy tài khoản nhận thanh toán hardhat, lưu lại địa chỉ deploy và thay vào contractaddress trong file app.js
- di chuyển tới folder frontend
- chạy npm install để cài đặt dependency
- chạy npm start

Cấu hình và link sản phẩm tới Metamask
- Lựa chọn mục network
- Chọn add network manually và thêm mạng localhost với RPC URL là http://localhost:8545 do Hardhat node được host mặc định tại port 8545
- Lựa chọn thêm Account, thêm account bằng private key được tạo bởi hardhat node
