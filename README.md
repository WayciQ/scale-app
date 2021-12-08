## Docker-compose.yml hiện tại đang cấu hình 3 service:
1. quanghoang0403/react-app: https://hub.docker.com/r/quanghoang0403/react-app 
2. quanghoang0403/api-server: https://hub.docker.com/r/quanghoang0403/api-server
3. mongo:3.6.19-xenial: https://hub.docker.com/layers/mongo/library/mongo/3.6.19-xenial/images/sha256-c0ae3888736d69a12caa6c43b40170b51425cfdf79fa3681f4540861576fce18?context=explore

## Có thể tự tạo 2 image react-app và api-server = Dockerfile như sau:
1. react-app
docker build -t "react-app" ./client/

2. api-server
docker build -t "api-server" ./server/

Sau khi tạo xong 2 image mới, nhớ sửa lại tên image trong docker-compose.yml
