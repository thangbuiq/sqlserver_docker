# `MSSQL_docker_compose`

> :bulb:This template is an example of an "push to GitHub" process document. You can reference and make your process document.

## :question: Dành cho ai
Dành cho những bạn không dùng Windows và muốn học SQL-Server, Repo này sẽ giúp các bạn sử dụng Image `sqlserver` trên **Docker** và host thông qua `localhost`. Từ đó, mọi người có thể connect trực tiếp thông qua SQL-Client như Azure Data Studio hay DBeaver.

## :feet: Step


1. Cài đặt docker và docker-compose, init sudo cho docker.
2. Mở Ctrl + Alt + T để mở Terminal lên và nhập lần lượt

```
git clone https://github.com/thangbuiq/sqlserver_docker.git
```
```
cd ./sqlserver_docker
```
```
make build
```
```
make up
```
Các bạn có thể thay đổi thông tin của mình trong file `docker-compose.yaml`:
- Username: không có khoảng cách, ký tự đặc biệt (Default: SA/sa)
- Password: 8 ký tự trở lên, có chữ hoa, số và ký tự đặc biệt. (Default: Ubunchuu@2022)
- Volume: thay đổi thông tin volume cần mount vào để chứa Database.
