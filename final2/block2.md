1.  **Lỗi triển khai thường gây lộ khóa riêng khi ký ECDSA là:**
    - Tái sử dụng hoặc dự đoán được nonce k (*)

2.  **Mục tiêu chính của đồng thuận trong blockchain là:**
    - Đảm bảo tất cả các node trong mạng phi tập trung đều thống nhất về cùng một trạng thái dữ liệu (ledger) — mà không cần bên thứ ba tin cậy.

3.  **Biện pháp nào giảm động lực tấn công 51% trong PoW?**
    - Tăng hashrate tổng thể phân tán và phần thưởng/penalty được thiết kế tốt ở lớp kinh tế

4.  **Trong over-collateralized lending, vị thế bị thanh lý khi:**
    - Tỷ lệ thế chấp rơi xuống dưới ngưỡng yêu cầu do giá biến động

5.  **Proof of Work (PoW) yêu cầu:**
    - Tính toán nặng để tìm băm thỏa target

6.  **Mục tiêu của inv/getdata (Bitcoin P2P) là:**
    - Trao đổi danh mục đối tượng (block/tx) và xin dữ liệu còn thiếu

7.  **PBFT phù hợp hơn với:**
    - Mạng permissioned có danh tính, số nút vừa phải

8.  **Trong quy trình ký ECDSA, dữ liệu nào được ký?**
    - Băm của thông điệp

9.  **Trong PoW, thợ đào thay đổi nonce để:**
    tìm hash nhỏ hơn target để giải khối

10. **Lưu dữ liệu lớn on-chain thường:**
    - Đắt; nên cân nhắc off-chain + hash/commit on-chain

11. **Trong block, Merkle root là:**
   Merkle root là băm tổng hợp của tất cả các giao dịch (transactions) trong block, được lưu trong block header.

12. **Cặp thuật toán bất đối xứng dùng phổ biến trong blockchain:**
    - ECDSA–secp256k1

13. **Impermanent loss xảy ra khi:**
    - Giá tài sản biến động so với thời điểm nạp thanh khoản, so với HODL

14. **Trong mô hình UTXO, đầu vào (input) của giao dịch tham chiếu:**
    
    - UTXO trước đó và cung cấp scriptSig/witness để chi tiêu

15. **Sau The Merge, Ethereum chuyển sang:**

    - PoS với validator, finality theo GHOST + Casper/FFG

16. **Trong PoW, target giảm kéo theo:**

    - Khó tìm block hơn, độ khó hiệu dụng tăng

17. **Latency mạng P2P tăng thường dẫn tới:**
    - Tỉ lệ fork/uncle tăng vì block truyền chậm


18. **Điểm khác biệt cốt lõi giữa mô hình trạng thái của Bitcoin và Ethereum là gì?**
  
    - Bitcoin dùng UTXO, Ethereum dùng mô hình account (account-based).

19. **Collision resistance giúp:**
    - Ngăn hai đầu vào cho cùng một băm khả dĩ trong thực tế


20. **Hai địa chỉ triển khai cùng một Solidity bytecode nhưng có khác nhau về:**
    - Code hash luôn giống, nhưng địa chỉ hợp đồng phụ thuộc nonce của deployer
    

21. **Rủi ro chính khi tái sử dụng địa chỉ/UTXO dễ nhận diện là:**

    - Tăng khả năng phân tích dòng tiền và liên kết danh tính on-chain

22. **Trade-off đúng giữa PoW vs PoS:**
    - PoW tiêu thụ năng lượng lớn, an ninh gắn với chi phí tính toán; PoS giảm năng lượng, an ninh gắn với stake và cơ chế kinh tế–xã hội


23. **Oracle risk trong DeFi chủ yếu đến từ:**

    - Phụ thuộc nguồn giá (manipulation, delay) dẫn đến thanh lý sai

24. **AMM constant product (x·y=k) có đặc điểm:**
    
    - Slippage tăng mạnh khi giao dịch lớn so với thanh khoản

25. **Gas trong EVM đo:**
  
    - Chi phí tính toán/lưu trữ theo opcode

26. **Ưu điểm của cấu trúc cây Merkle so với danh sách tuyến tính:**
    - cho phép chứng minh thành viên nhanh

27. **Trong PoS hiện đại (VD: Ethereum), cơ chế slashing dùng để:**
   
    - Phạt validator hành vi xấu (double-sign, không trung thực)

28. **Hàm băm “nhạy cảm đầu vào” (avalanche effect) mô tả:**
    Đầu vào đổi 1 bit → đầu ra đổi mạnh toàn bộ

29. **Hardware wallet giúp tăng an toàn vì:**
    - Lưu khóa riêng và ký trong phần cứng, không lộ ra hệ điều hành
   

30. **Orphan/uncle block thường sinh ra khi:**
    - Hai miner cùng tìm được block hợp lệ gần như đồng thời
    

31. **Delegatecall nguy hiểm nếu:**

    - Nó thực thi code của hợp đồng khác trong context storage của caller

32. **Ưu điểm của Merkle tree so với băm tuyến tính danh sách:**
  
    - Cho phép chứng minh thành viên nhanh và nhỏ gọn

33. **Cơ chế chống eclipse attack hiệu quả hơn là:**
   
    - Duy trì nhiều kết nối ra/vào, đa dạng nguồn peer và kiểm soát bảng peer

34. **Địa chỉ blockchain (ví dụ Bitcoin/Ethereum) thường:**
    
    - Là mã hóa của khóa công khai/seed phrase

35. **Lý do chính khiến tấn công 51% nguy hiểm trong chuỗi PoW:**
    - Kẻ tấn công có thể tạo chuỗi dài hơn để double-spend và tái tổ chức lịch sử gần
  

36. **Proof of Stake (PoS) cơ bản chọn người xác thực dựa trên:**
    - Số lượng coin/stake
37. **“Dust limit” liên quan đến:**

    - Ngưỡng giá trị UTXO quá nhỏ, chi tiêu không kinh tế do phí

38. **Merkle root thay đổi khi:**
    - Sắp xếp giao dịch khác đi (trong cùng tập)


39. **Chức năng chính của khóa công khai trong chữ ký số:**
    - Xác minh chữ ký


40. **Một tấn công làm sai Merkle tree nhưng vẫn giữ nguyên root là:**
    - Không thể nếu dùng băm an toàn và cấu trúc đúng
    

41. **Tính chất “không chối bỏ” (non-repudiation) đến từ:**
    - Chữ ký số bằng khóa riêng
   
42. **Tham số nào không trực tiếp thuộc header trong Bitcoin?**
  
      

43. **Flash loan thích hợp để:**
 
    - Thực hiện arbitrage/hoán đổi/tái cấp vốn trong một giao dịch nguyên tử

44. **Sự khác nhau chính giữa storage và memory trong Solidity:**
   
    - storage bền vững on-chain (đắt), memory tạm thời trong call (rẻ hơn)

45. **Trong mạng permissioned, đồng thuận hay dùng:**
    - PBFT/Raft và biến thể
    

46. **Ưu thế của gossip protocol trong mạng blockchain là:**
  
    - Phân tán thông tin nhanh, chịu lỗi tốt mà không cần trung tâm

47. **Vì sao elliptic-curve (ECDSA/EdDSA) thường được ưa chuộng hơn RSA trên chuỗi?**
    
    - Cùng mức an toàn với kích thước khóa nhỏ hơn, hiệu năng tốt

48. **Vì sao không nên dùng SHA-256 cho lưu mật khẩu người dùng?**
   
    - Vì không chậm và không có muối (salt) theo thiết kế; nên dùng bcrypt/Argon2/scrypt

49. **Merkle proof cho phép:**
    - Xác minh một giao dịch thuộc khối với bằng chứng ngắn, không cần toàn bộ danh sách giao dịch
 

50. **Ưu điểm của UTXO đối với song song hóa xác minh (parallel validation):**

    - Đầu vào độc lập cho phép xác minh song song các giao dịch không đụng UTXO

51. **Một hàm băm mật mã dùng rộng rãi trong blockchain:**
  
    - SHA-256

52. **Thuộc tính preimage resistance nghĩa là:**

    - Khó tìm đầu vào từ đầu ra

53. **Thiết lập mining pool chủ yếu để:**

    - Chia sẻ rủi ro biến động phần thưởng và làm mượt doanh thu

54. **“Băm một chiều” nghĩa là:**

    - Dễ tính băm, khó tìm ngược đầu vào từ băm

55. **Lý do Ethereum cần nonce trong mỗi tài khoản là:**
  
    - Tránh replay giao dịch và xác định thứ tự giao dịch của tài khoản

56. **Mã khóa bất đối xứng sử dụng hai loại khóa:**

    - Khóa công khai và khóa bí mật

57. **Phát biểu đúng về multi-signature (multisig):**
    - Cho phép nhiều bên cùng sinh một khóa riêng


58. **Trong khối block, Merkle root là:**
- Băm tổng hợp tất cả giao dịch trong block, lưu trong header
