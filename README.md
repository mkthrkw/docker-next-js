# docker for next.js

## プロジェクト作成

### 1. 下記ファイルを作成する
* docker-compose.yml
* .env

### ２. コンテナを作成しておく
```shell:
docker compose up -d
```

### ３. アプリインストール

#### Next.js
```shell:
docker compose run --rm next sh -c 'npx create-next-app@latest .'
```

#### T3 stack
```shell:
docker compose run --rm next sh -c 'npm create t3-app@latest .'
```

### ４. コンテナを起動
```shell:
docker compose up -d
```

### ５. ローカルホストへアクセス
http://localhost:3000
