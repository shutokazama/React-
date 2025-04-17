# Node.jsの公式イメージを使用
FROM node:22

# 作業ディレクトリ作成
WORKDIR /app

# 依存ファイルをコピー
COPY package*.json ./
COPY tsconfig.json ./
COPY vite.config.ts ./

# 依存関係をインストール
RUN npm install

# ソースコードをコピー
COPY . .

# 開発サーバーを起動（ポートはViteのデフォルト：5173）
CMD ["npm", "run", "dev"]
