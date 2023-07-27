# 概要
- Allegro 開発効率化WGの活動の一貫として、CI/CDなど導入障壁の軽減​のため、CI/CD Startkitを提供する
- GitHub ActionsをはじめとしたCI/CDがすぐに利用できるようなリポジトリを整備し、GitHub Template RepositoryとしてSSS Organization内の誰もが利用できるようにする

# 実現したいこと
- TemplateリポジトリをForkすると、Forkしたリポジトリでプロジェクトの担当者が以下の機能をすぐに利用できるようになっていること
- TemplateリポジトリはSSS Organization全てのエンジニアがcontribute可能になっていること
  - 各プロジェクトの熱意あるエンジニア達が、誰でも共通基盤としてTemplateリポジトリを改善できるようにする

# 機能
## CI
- `Pull Request`作成時にGitHub ActionsでUnit Testが実行される
- `main`ブランチへのマージ後にGitHub ActionsでUnit Testが実行される

## CD
- `main`ブランチへのマージ後にGitHub ActionsでDocker buildが実行されて、リモートリポジトリへPushされる

## 開発環境
- `.devcontaienr`を利用した、エンジニアが共通利用できるローカル開発環境の提供 