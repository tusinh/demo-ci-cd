# install jenkin docker
docker run -d \
  --name jenkins \
  -p 8080:8080 \
  -p 50000:50000 \
  jenkins/jenkins:lts

# ACC jenkin
- passJenkins (admin): bff21651d33c40efaadad21f8fedc91e
- username: cautu
- pass: cautu123
- email: cautu404@gmail.com



# Demo CI/CD với GitHub Actions

## Mô tả
Repo này chứa app Node.js đơn giản (hàm sum) và test bằng Jest.  
CI pipeline chạy với GitHub Actions gồm các bước:
1. Checkout code
2. Cài dependency
3. Build app
4. Run test

## Kết quả
- Khi push code lên `main`, pipeline tự động chạy.
- Nếu test pass → pipeline xanh.
- Nếu test fail → pipeline đỏ.
