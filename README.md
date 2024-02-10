# Rust Sample API

## 準備

```bash
cat <<EOF > .env
DB_NAME=rust_sample
DB_USER=rust_user
DB_PASS=rust_pass
DB_PORT=3306
MYSQL_ROOT_PASSWORD=root
TZ=Asia/Tokyo
EOF
```

## 実行

```bash
docker compose up
```

## DBの初期化

```bash
docker volume rm rust_sample_api_db-vol
docker compose down
docker compose up --build
```
