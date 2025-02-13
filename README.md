# nuxt3-sample

export DOCKER_BUILDKIT=0
docker-compose build --no-cache
docker-compose up -d

# docker内部にログイン
docker-compose exec sample-nuxt sh

# docker内部にログインして初回プロジェクト作成
npx nuxi@latest init

# 以下を実行してサーバー起動
npm run dev

# 表示確認
http://localhost:3100/

# docker内部で必要なものをinstall
# npm install ライブラリ名 --save
# 開発環境のみに必要な場合は以下
# npm install ライブラリ名 --save-dev
