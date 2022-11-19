# 業務経歴書

## 基本情報

株式会社 premices 代表 藤川 慶

Web サービス・モバイルアプリの開発支援を行なっています。

### 略歴

東京大学教養学部卒、2019 年よりエンジニアとしてキャリアスタート。ベンチャー企業に正社員として 2 年間勤務したのちフリーランスとして独立。現在は株式会社 premices を設立し、Web サービスやモバイルアプリ開発の支援を行なっている。

### 各種 SNS アカウント

|          | URL                                            |
| -------- | ---------------------------------------------- |
| GitHub   | [@keiffff](https://github.com/keiffff)         |
| Twitter  | [@kei_ffff](https://twitter.com/kei_ffff)      |
| Wantedly | [keiffff](https://www.wantedly.com/id/keiffff) |

## 業務経歴

### B to B メーカー・物流業界向けデータ開示サービス（Web）の新規開発（2022 年 4 月 ~ ）

#### 概要

4 名からなるチームの開発リードを担当。要件定義・画面設計・DB 設計・アーキテクチャ設計・コード基盤の実装・テスト・運用について担当。

#### 担当業務

- Web フロントエンドに必要な各種バックエンドサービスへのアクセスを集約するための GraphQL BFF を実装。スキーマ駆動による高い生産性と型安全性を担保した開発を実現。
- Hasura を導入することで、データ格納先である BigQuery や PostgreSQL に対し、安全性・柔軟性の高いデータアクセスを実現。
- React + TypeScript + Apollo Client を活用したフロントエンドの実装。
- ベースとなる UI コンポーネントの設計・実装。Storybook を活用してコンポーネント単位での開発を実現する仕組みの構築。
- Cloud Load Balancer + App Engine を活用したフロントエンド配信基盤の構築。
- Cloud Run を活用したサーバーレスバックエンドサービスの構築。
- 外部ベンダー提供の認証用 API + Cloud Memorystore（Redis）によるセッション永続化 + Cookie を活用した認証機能の実装。CSRF 脆弱性を含めた各種脆弱性についての対策も実施。
- Cloud Run から VPC 上に配置された Cloud Memorystore（Redis）へアクセスを行うためのサーバーレスアクセスコネクタを導入。
- Cloud Tasks を活用した数十万件程度のレコードの取得・集計を行うジョブの非同期化。
- Cloud Logging を活用し、障害時に追跡がしやすいようアプリケーションから JSON で構造化されたログを出力する仕組みを実装。
- Secret Manager を活用した秘匿情報の管理。CloudBuild でのアプリケーションのビルド時に秘匿情報を環境変数として注入する仕組みの構築。
- SendGrid を活用したメール配信基盤の構築。
- docker-compose を活用したローカル開発基盤の構築。
- Bitbucket Pipelines を活用した CI パイプラインの構築。プルリクエスト単位でコードの静的解析・単体テストを自動で実行する仕組みを実現。
- CloudBuild を活用した CD パイプラインの構築。各種サービスのデプロイ自動化、DB マイグレーションの自動化を実現。
- 開発中の動作を確認するためのステージング環境を構築。組織外からのアクセスを防ぐ目的のため、Cloud Load Balancer に対して Cloud IAP による Google アカウント認証を設けることで、簡易的かつセキュアなアクセス制限を実現。
- 他メンバーの設計レビュー・コードレビュー・メンタリング業務を担当。

#### 発揮したバリュー

開発リードとして開発初期から参画。プロダクトオーナーとの打ち合わせに参加し、要件定義を実施。コンテキスト図やユースケース図を活用しながら、当該サービスを用いることによる顧客の業務フローとサービスの創出価値について整理。要件を基に作成したワイヤーフレーム図をプロダクトオーナーに提案し、サービスイメージの認識合わせを行うなど上流工程から貢献。早い段階からデプロイ自動化やステージング環境の構築を実施することで、プロダクトオーナーに都度成果物を確認してもらいながらフィードバックを得やすい体制づくりに貢献。サービスの要件上、数十万件程度のレコードの入出力を必要としていたため、GCP の各種マネージドサービスの制限に引っかかることのないよう実装面でも工夫を施していた。

### B to B メーカー・物流業界向け情報分析サービス（Web）の新規開発（2021 年 11 月 ~ ）

#### 概要

2 名からなるチームの開発リードを担当。要件定義・画面設計・アーキテクチャ設計・コード基盤の実装・テスト・運用について担当。

#### 担当業務

- Web フロントエンドに必要な各種バックエンドサービスへのアクセスを集約するための GraphQL BFF を実装。スキーマ駆動による高い生産性と型安全性を担保した開発を実現。
- React + TypeScript + Apollo Client を活用したフロントエンドの実装。
- ベースとなる UI コンポーネントの設計・実装。Storybook を活用してコンポーネント単位での開発を実現する仕組みの構築。
- recharts を活用したフロントエンドでのデータビジュアライズ機能の実装。
- Cloud Load Balancer + App Engine を活用したフロントエンド配信基盤の構築。
- Cloud Run を活用したサーバーレスバックエンドサービスの構築。
- Cloud Logging を活用し、障害時に追跡がしやすいようアプリケーションから JSON で構造化されたログを出力する仕組みを実装。
- Cloud Scheduler + Cloud Tasks + Cloud Run を活用した、ユーザーごとの指定時刻におけるメール自動配信機能の実装。
- Secret Manager を活用した秘匿情報の管理。CloudBuild でのアプリケーションのビルド時に秘匿情報を環境変数として注入する仕組みの構築。
- SendGrid を活用したメール配信基盤の構築。
- アクセス可能なユーザーを契約済みの顧客のみに制限するため、Cloud Load Balancer に対して Cloud IAP による Google アカウント認証を設けることで、簡易的かつセキュアなアクセス制限を実現。
- Bitbucket Pipelines を活用した CI パイプラインの構築。プルリクエスト単位でコードの静的解析・単体テストを自動で実行する仕組みを実現。
- CloudBuild を活用した CD パイプラインの構築。各種サービスのデプロイ自動化を実現。

#### 発揮したバリュー

開発リードとして開発初期から参画。デザイナー不在のプロジェクトであったため、要件を整理し、他社のサービスを参考にアプリケーションとして使いやすい UI を模索し提案するなど上流工程から貢献。外部 API の返す結果を一定程度複雑な要件のもとビジュアライズ化する必要があったが難なくクリア。ユーザーごとの指定時刻におけるメール配信といった要件についても、これまでの業務経験を活かし短期間で対応。

### B to C 店舗型ショッピングアプリ（iOS・Android）の POC 開発（2021 年 5 月 ~ 2021 年 10 月）

#### 概要

1 名からなるチームの開発リードを担当。要件定義・アーキテクチャ設計・コード基盤の実装・テストについて担当。

#### 担当業務

- Web フロントエンドに必要な各種バックエンドサービスへのアクセスを集約するための GraphQL BFF を実装。スキーマ駆動による高い生産性と型安全性を担保した開発を実現。
- ReactNative（Expo）を活用した iOS・Android 両対応のアプリを実装。
- ベースとなる UI コンポーネントの設計・実装。Storybook を活用してコンポーネント単位での開発を実現する仕組みの構築。
- Expo のリリースチャンネルを活用し、開発中の動作を確認するためのステージング環境を構築。Expo の organization 管理下にある社内アカウントにのみアプリを配信可能な仕組みを構築。
- Cloud Run を活用したサーバーレスバックエンドサービスの構築。
- Cloud Logging を活用し、障害時に追跡がしやすいようアプリケーションから JSON で構造化されたログを出力する仕組みを実装。
- 外部ベンダー提供の認証用 API からアクセストークン・リフレッシュトークンを取得し、デバイス上のストアに暗号化して保存。トークンをローテーションすることでセキュアに認証情報を保持する仕組みを実装。
- Secret Manager を活用した秘匿情報の管理。CloudBuild でのアプリケーションのビルド時に秘匿情報を環境変数として注入する仕組みの構築。
- Bitbucket Pipelines を活用した CI パイプラインの構築。プルリクエスト単位でコードの静的解析・単体テストを自動で実行する仕組みを実現。
- CloudBuild を活用した CD パイプラインの構築。各種サービスのデプロイ自動化を実現。

#### 発揮したバリュー

開発リードとして開発初期から参画。既に Web サービスとして利用されているプロダクトのモバイルアプリ企画であったが、モバイルアプリ開発経験を有する開発メンバーが不在という状況であった。モバイルアプリにおける各種ガイドラインのキャッチアップ、Web アプリ版を利用するユーザーとのメンタルモデルの差異といった詳細について検討を行い、主体的に機能仕様や画面設計について提言を行なっていた結果、プロダクトオーナーの判断上モバイルアプリとして不自由ない操作性を実現。スワイプやピンチ & ズームによる操作、Web コンテンツの埋め込みといったモバイルアプリ特有の要件についてもクリア。

### B to B 法務系サービス（Web）の開発（2020/6 月 ~ 2021/5 月）

#### 概要

5 ~ 12 名程度からなるチームにおいて正社員メンバーとして要件定義・設計・開発・テスト・運用について担当。

#### 担当業務

- React + TypeScript を活用したフロントエンドの実装。
- Cloud Functions + Firebase を活用したサーバーレスバックエンドサービスの構築。
- Cloud Scheduler + Cloud Functions を活用したデータベースの定期自動バックアップ機能を実装。
- Firebase Auth・Cloud Firestore を活用したユーザー一括登録スクリプトを実装。
- Google Tag Manager を活用したアクセス解析用データのアプリケーションへの組み込みを実装。
- 数万 ~ 数十万件程度のレコードを処理するための各種バッチ処理を実装。

#### 発揮したバリュー

ベータ版のサービスから正社員メンバーとしてプロジェクトへ参画。ビジネスインパクトの大きな機能の開発を担当し、サービスの正式版リリースへ貢献した。新規機能の実装だけでなく、増加する利用者数に伴うボトルネックの解消や障害対応といった運用面での課題解決にも主体的にコミットし、プロダクトの拡大に貢献した。メンバーの採用活動や、新規メンバーへのオンボーディング、チームファシリテーション、開発用ドキュメントの作成なども主体的に行い、主力メンバーとしてチーム強化に貢献した。
