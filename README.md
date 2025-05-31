# なにこれー？

- Render へのデプロイを試した際のダミーアプリです
- https://render-deploy-w0y2.onrender.com/
- 2025.05.30 時点で、マルチコンテナ構成はそのままデプロイ不可で、各々を別サービスとして登録する必要があるそうです
  - DB を単独サービスとして登録すると、Rrender 内に環境変数 `DATABASE_URL` が登録され、別サービスから参照可能になります
  - AWS CDK のような IaC(Infrastructure as Code) ツールとして `Render Blueprints` (render.yaml) があります
