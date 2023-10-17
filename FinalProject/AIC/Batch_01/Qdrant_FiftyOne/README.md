# Hướng dẫn chạy thực nghiệm Qdrant - FiftyOne

1. Cài docker desktop về máy tại đường dẫn: https://docs.docker.com/get-docker/ 

2. Mở docker desktop

Chạy các lệnh sau trong terminal tại thư mục đang làm việc:

3. Pull qdrant về: ```docker pull qdrant/qdrant```

4. Chạy qdrant vừa pull về: ```docker run -p 6333:6333 qdrant/qdrant```

5. Mở ```http://localhost:6333``` để set api key

6. Copy API và dán vào các vị trí khai báo api_key

4. Mở tệp Qdrant_FiftyOne.ipynb chứa code bằng Visual Studio Code

5. Chọn kernel thích hợp

6. Chọn Run các cell 

7. Thay đổi câu query và thực hiện truy vấn