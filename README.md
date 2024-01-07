# docker for next.js

### 初期プロジェクト作成
#### 1. 下記ファイルを作成する
* docker-compose.yml
* Dockerfile
* .env

#### 2. プロジェクト作成のため、docker-compose.yml内の下記をコメントアウト
```
    # command: npm run dev ←コレ
```

#### 3. コンテナ起動する
```
docker compose up -d
```

#### 4. 起動時に作成されたホスト側./src/node_moduleディレクトリを削除

#### 5. コンテナに入る
```
docker compose exec -it next sh
```

#### 6. 公式ドキュメントに従ってインストール
https://nextjs.org/docs/getting-started/installation  
```npx create-next-app@latest```

#### 7. コンテナから一度出る
```exit```

#### 8. 上記2でコメントアウトしたcommandを有効にする
```
    command: npm run dev ←コレ
```

#### 9. コンテナを再作成
```
docker compose up -d
```

#### 10. ローカルホストへアクセス
http://localhost:3000