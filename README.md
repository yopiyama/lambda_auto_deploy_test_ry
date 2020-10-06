# lambda_auto_deploy_test_ry

Github Actions を使った AWS Lambda への自動デプロイを試すレポ

Master と Develop ブランチへプッシュした際に自動的に AWS Lambda へデプロイされる

## ファイルについて

デプロイなどの処理を行っているスクリプトは **lambda_auto_deploy_test_ry/.github/workflows/deploy_XXXXXX.yml**

Master ブランチへの Push を検知した場合は、**deploy_master.yml**、Develop ブランチへの Push を検知した場合は **deploy_develop.yml** が動作する。  
また、特定のパス（test-function/*）で変更があった場合動作するという条件をつけてある。
