## Docker-compose.yml hiện tại đang cấu hình 3 service:
1. quanghoang0403/react-app: https://hub.docker.com/r/quanghoang0403/react-app 
2. quanghoang0403/api-server: https://hub.docker.com/r/quanghoang0403/api-server
3. mongo:3.6.19-xenial: https://hub.docker.com/layers/mongo/library/mongo/3.6.19-xenial/images/sha256-c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18?context=explore

## Run Docker-compose
Mở terminal scale-app-master, run

`docker-compose up`

Sau khi run 3 container đã được chạy, có thể mở Docker Desktop để kiểm tra

## Có thể tự tạo 2 image react-app và api-server = Dockerfile như sau:
1. react-app

Mở terminal scale-app-master, run

`docker build -t "react-app" ./client/`

2. api-server

Mở terminal scale-app-master, run

`docker build -t "api-server" ./server/`

Sau khi tạo xong 2 image mới, nhớ sửa lại tên image trong docker-compose.yml để run multi container theo 2 image vừa mới tạo
