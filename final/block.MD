1.   Trong mô hình UTXO, đầu vào (input) của giao dịch tham chiếu:
    - Số dư tài khoản
    - UTXO trước đó và cung cấp scriptSig/witness để chi tiêu

2.   Flash loan thích hợp để:
    - Vay dài hạn
    - Thực hiện arbitrage/hoán đổi/tái cấp vốn trong một giao dịch nguyên tử

3.   Mục tiêu của inv/getdata (Bitcoin P2P) là:
    - Thương lượng phí
    - Trao đổi danh mục đối tượng (block/tx) và xin dữ liệu còn thiếu

4.   Hai địa chỉ triển khai cùng một Solidity bytecode nhưng có khác nhau về:
    - Code hash luôn giống, nhưng địa chỉ hợp đồng phụ thuộc nonce của deployer
    - Code hash khác nhau

5.   Impermanent loss xảy ra khi:
    - Giá tài sản không đổi
    - Giá tài sản biến động so với thời điểm nạp thanh khoản, so với HODL

6.   AMM constant product (x·y=k) có đặc điểm:
    - Giá tuyến tính theo khối lượng
    - Slippage tăng mạnh khi giao dịch lớn so với thanh khoản

7.   Lỗi triển khai thường gây lộ khóa riêng khi ký ECDSA là:
    - Dùng băm SHA-256
    - Tái sử dụng hoặc dự đoán được nonce k

8.   Hàm băm “nhạy cảm đầu vào” (avalanche effect) mô tả:
    - Đầu vào đổi 1 bit → đầu ra đổi nhỏ
    - Đầu vào đổi 1 bit → đầu ra đổi lớn và khó dự đoán

9.   Ưu điểm của UTXO đối với song song hóa xác minh (parallel validation):
    - Khó tách biệt phụ thuộc
    - Đầu vào độc lập cho phép xác minh song song các giao dịch không đụng UTXO

10.  Sự khác nhau chính giữa storage và memory trong Solidity:
    - Cả hai đều volatile
    - storage bền vững on-chain (đắt), memory tạm thời trong call (rẻ hơn)

11.  Mục tiêu chính của đồng thuận trong blockchain là:
    - Tăng màu sắc giao diện
    - Tất cả nút đồng ý cùng một trạng thái sổ cái

12.  Một hàm băm mật mã dùng rộng rãi trong blockchain:
    - MD5
    - SHA-256

13.  Cặp thuật toán bất đối xứng dùng phổ biến trong blockchain:
    - ECDSA–secp256k1
    - RSA–SHA1

14.  Mã khóa bất đối xứng sử dụng hai loại khóa:
    - Hai khóa bí mật giống nhau
    - Khóa công khai và khóa bí mật

15.  Tính chất “không chối bỏ” (non-repudiation) đến từ:
    - Chữ ký số bằng khóa riêng
    - Hàm băm

16.  Trong khối block, Merkle root là:
    - Băm của header
    - Băm tổng hợp của cây băm các giao dịch

17.  “Băm một chiều” nghĩa là:
    - Băm rồi có thể giải ngược
    - Dễ tính băm, khó tìm ngược đầu vào từ băm

18.  Hardware wallet giúp tăng an toàn vì:
    - Lưu khóa riêng và ký trong phần cứng, không lộ ra hệ điều hành
    - Không cần PIN

19.  Điểm khác biệt cốt lõi giữa mô hình trạng thái của Bitcoin và Ethereum là gì?
    - Bitcoin dùng account, Ethereum dùng UTXO
    - Cả hai đều dùng UTXO

20.  Trade-off đúng giữa PoW vs PoS:
    - PoW tiêu thụ năng lượng lớn, an ninh gắn với chi phí tính toán; PoS giảm năng lượng, an ninh gắn với stake và cơ chế kinh tế–xã hội
    - PoW luôn nhanh hơn PoS

21.  Thuộc tính preimage resistance nghĩa là:
    - Khó tìm hai đầu vào khác nhau cho cùng đầu ra
    - Khó tìm đầu vào tương ứng với một giá trị băm cho trước

22.  Collision resistance giúp:
    - Ngăn hai đầu vào cho cùng một băm khả dĩ trong thực tế
    - Ngăn mọi va chạm tuyệt đối về mặt toán học

23.  Trong over-collateralized lending, vị thế bị thanh lý khi:
    - Tỷ lệ thế chấp vượt ngưỡng an toàn
    - Tỷ lệ thế chấp rơi xuống dưới ngưỡng yêu cầu do giá biến động

24.  Lý do chính khiến tấn công 51% nguy hiểm trong chuỗi PoW:
    - Kẻ tấn công có thể tạo chuỗi dài hơn để double-spend và tái tổ chức lịch sử gần
    - Không ảnh hưởng gì

25.  Lý do Ethereum cần nonce trong mỗi tài khoản là:
    - Đếm số block đã đào
    - Tránh replay giao dịch và xác định thứ tự giao dịch của tài khoản

26.  Event logs trên EVM chủ yếu để:
    - Lưu state chính
    - Ghi log rẻ hơn storage và dùng cho indexing ngoài chuỗi (không thay thế state)

27.  Phát biểu đúng về multi-signature (multisig):
    - Cho phép nhiều bên cùng sinh một khóa riêng
    - Yêu cầu ngưỡng chữ ký (m-of-n) để chi tiêu giao dịch

28.  Proof of Work (PoW) yêu cầu:
    - Bỏ qua băm
    - Tính toán nặng để tìm băm thỏa target

29.  Proof of Stake (PoS) cơ bản chọn người xác thực dựa trên:
    - Băng thông mạng
    - Lượng stake và/hoặc các tiêu chí ngẫu nhiên có trọng số

30.  Chức năng chính của khóa công khai trong chữ ký số:
    - Xác minh chữ ký
    - Tạo chữ ký

31.  Trong quy trình ký ECDSA, dữ liệu nào được ký?
    - Bản rõ nguyên vẹn
    - Băm của thông điệp

32.  Lý do địa chỉ nhận thay đổi (change address) thường khác địa chỉ gửi:
    - Bảo mật/riêng tư tốt hơn và chuẩn ví
    - Bắt buộc bởi giao thức

33.  Oracle risk trong DeFi chủ yếu đến từ:
    - Không có hợp đồng
    - Phụ thuộc nguồn giá (manipulation, delay) dẫn đến thanh lý sai

34.  Gas trong EVM đo:
    - Dung lượng RAM
    - Chi phí tính toán/lưu trữ theo opcode

35.  Trong PoW, target giảm kéo theo:
    - Dễ tìm block hơn
    - Khó tìm block hơn, độ khó hiệu dụng tăng

36.  Lưu dữ liệu lớn on-chain thường:
    - Rẻ và khuyến khích
    - Đắt; nên cân nhắc off-chain + hash/commit on-chain

37.  Thiết lập mining pool chủ yếu để:
    - Giảm xác suất tìm block
    - Chia sẻ rủi ro biến động phần thưởng và làm mượt doanh thu

38.  Ưu điểm của Merkle tree so với băm tuyến tính danh sách: (Hoặc: Ưu điểm của cấu trúc cây Merkle so với danh sách tuyến tính:)
    - Dễ đảo ngược / Tăng kích thước lưu trữ
    - Cho phép chứng minh thành viên nhanh và nhỏ gọn / Loại bỏ nhu cầu băm

39.  Latency mạng P2P tăng thường dẫn tới:
    - Tỉ lệ fork/uncle tăng vì block truyền chậm
    - Tỉ lệ fork giảm

40.  Orphan/uncle block thường sinh ra khi:
    - Hai miner cùng tìm được block hợp lệ gần như đồng thời
    - Node lỗi đồng bộ

41.  Trong mạng permissioned, đồng thuận hay dùng:
    - PBFT/Raft và biến thể
    - PoW thuần

42.  PBFT phù hợp hơn với:
    - Mạng permissioned có danh tính, số nút vừa phải
    - Mạng công khai vô danh quy mô cực lớn

43.  Rủi ro chính khi tái sử dụng địa chỉ/UTXO dễ nhận diện là:
    - Giảm fee
    - Tăng khả năng phân tích dòng tiền và liên kết danh tính on-chain

44.  Sau The Merge, Ethereum chuyển sang:
    - PoW + Ethash
    - PoS với validator, finality theo GHOST + Casper/FFG

45.  Merkle root thay đổi khi:
    - Sắp xếp giao dịch khác đi (trong cùng tập)
    - Thay đổi nonce khối

46.  “Dust limit” liên quan đến:
    - Kích thước block tối đa
    - Ngưỡng giá trị UTXO quá nhỏ, chi tiêu không kinh tế do phí

47.  Tham số nào không trực tiếp thuộc header trong Bitcoin?
    - Version
    - Gas price

48.  Tối ưu gas khi lập trình EVM không nên:
    - Dùng calldata cho tham số chỉ đọc trong external function
    - Gộp/pack biến uint256 không liên tiếp vào cùng slot khi hợp lý

49.  Ưu thế của gossip protocol trong mạng blockchain là:
    - Đảm bảo thông điệp đến đích duy nhất
    - Phân tán thông tin nhanh, chịu lỗi tốt mà không cần trung tâm

50.  Vì sao không nên dùng SHA-256 cho lưu mật khẩu người dùng?
    - Vì không an toàn mật mã
    - Vì không chậm và không có muối (salt) theo thiết kế; nên dùng bcrypt/Argon2/scrypt

51.  Trong PoS hiện đại (VD: Ethereum), cơ chế slashing dùng để:
    - Tăng phần thưởng
    - Phạt validator hành vi xấu (double-sign, không trung thực)

52.  Trong PoW, difficulty adjustment (VD: Bitcoin 2016 block) để:
    - Giữ thời gian block trung bình ổn định (VD: ~10 phút)
    - Tăng phí

53.  Một tấn công làm sai Merkle tree nhưng vẫn giữ nguyên root là:
    - Không thể nếu dùng băm an toàn và cấu trúc đúng
    - Luôn có thể