# Resume

* [GitHub Pages link](https://d-kuro.github.io/resume/)

## Personal Information

| key  | value |
| - | - |
| Name | Dai Kurosawa |
| Sex | 男 |
| Age | 24 |
| Mail | [kurosawa7620@gmail.com](mailto:kurosawa7620@gmail.com) |
| Twitter | [@ponde_m](https://twitter.com/ponde_m) |
| GitHub | [@d-kuro](https://github.com/d-kuro) |
| Blog 1 | [d-kuro.github.io/record](https://d-kuro.github.io/record) |
| Blog 2 | [あふん](https://ponde-m.hatenablog.com/) |
| Company Blog | [黒澤大 ｜ DevelopersIO](https://dev.classmethod.jp/author/kurosawa-dai/)|

## 自然言語

| 自然言語 | 備考                                  |
| ------ | ------------------------------------- |
| 日本語  | ネイティブ                              |
| 英語    | 英語で書かれた文書を Google 翻訳や辞書を使いつつ、理解することができる |

## 技術スタック

* Go
  * 主にツール, Docker コンテナで実行するアプリケーションの開発に使用
  * プライベートで書いてるのは基本 Go
* Kubernetes
  * Microservice を動作させる基盤として Amazon ECS から Amazon EKS への移行作業を実施中
  * Argo CD を用いた GitOps を実践しており, 周辺のエコシステムに関してもキャッチアップを行なっている
  * 基本的な manifest の記述から, 必要に応じてソースコードの読み込みまでやっている
  * clinet-go を用いた小さめのアプリケーションを開発, 今後は Operator の作成等を経験していきたい
* Java
  * Spring Boot を用いたアプリケーションの開発を2年程度

## 興味 & 関心

* SaaS 開発
* Kubernetes を用いた Microservice 環境化 SRE として組織生産性を高めるための仕組みづくりをしていきたい
  * Microservice という複雑な環境下で Microservice のチーム単位でオーナシップを持ち Dev から Ops まで回していけるような仕組みづくり 
  * Operator とかの開発もしていきたい
* プログラミング言語は Go を使いたい
  * シングルバイナリになることからのツール開発等での相性の良さ
  * Kubernetes, Docker 等のコンテナ界隈での採用率

## 目標

### 短中期目標

* OSS 活動
* Kubernetes 界隈での情報のキャッチアップ, 率先してキャッチアップした情報を発信する
* [CKA (Certified Kubernetes Administrator)](https://www.cncf.io/certification/cka/) と [CKAD (Certified Kubernetes Application Developer)](https://www.cncf.io/certification/ckad/) の取得
* 英会話と英作文の学習をすること
  * レアジョブを始めた
* イベント等で LT 枠以外の登壇をすること

### 長期目標

* 英語を用いた業務対応やカンファレンス等での英語を用いた質疑応答ができるようになること
* リーダ職について技術だけでなくチームビルディングにおいてもバリューを出すこと

## 労働環境に関する希望

* 技術力向上がしやすい環境
  * 技術力向上に対する意欲の高い人が多い
  * モダンな技術に挑戦できる
  * 勉強会, 企業ブログ等で外部へのアウトプットを行なっている
  * 業務時間内でのカンファレンス参加等が認められている
  * 書籍購入費, カンファレンス参加費, 資格試験費などがある程度補助される
* フレックス制度
  * ある程度自分の裁量で就業時間をコントロールでき, 勉強会などに参加しやすい環境

## 資格

| 取得時期 | 資格名 |
| - | - |
| 2012/11 | ITパスポート試験 |
| 2013/11 | 基本情報技術者試験 |
| 2014/12 | 応用情報技術者試験 |
| 2015/06 | 情報セキュリティスペシャリスト試験 |
| 2016/06 | データベーススペシャリスト試験 |
| 2016/12 | ネットワークスペシャリスト試験 |
| 2018/05/30 | AWS Certified Solutions Architect - Associate Level |
| 2018/06/18 | AWS Certified Developer - Associate Level |
| 2018/06/27 | AWS Certified SysOps Administrator - Associate Level |

## Speaker

* 20180918
  * [Gopher道場#3 卒業式＆LT大会](https://mercari.connpass.com/event/101178/)
  * [Go Cloud を触ってみる / gopher-dojo-lt](https://speakerdeck.com/daikurosawa/gopher-dojo-lt)
* 20181214
  * [Introduction gRPC](https://speakerdeck.com/daikurosawa/introduction-grpc)
* 20180131
  * [Go(Un)Conference（Goあんこ）LT大会 5kg](https://gounconference.connpass.com/event/112942/)
  * [GolangCI を使ってコードの品質を保ちながら快適な Golang 生活を送る話 #gounco / GolangCI - Speaker Deck](https://speakerdeck.com/daikurosawa/golangci)
* 20190527
  * [Go(Un)Conference（Goあんこ）LT大会 6kg](https://gounconference.connpass.com/event/129090/)
  * [Kubernetes のソースコードとの付き合い方 #gounco / Kubernetes source code reading](https://speakerdeck.com/daikurosawa/kubernetes-source-code-reading)
* 20190531
  * [Kubernetes Meetup Tokyo 19 (Yahoo! JAPAN MEETUP共催)](https://k8sjp.connpass.com/event/126207/)
  * [図で理解する Descheduler #k8sjp #ymju / Introduction to Descheduler](https://speakerdeck.com/daikurosawa/introduction-to-descheduler)

## 職務経歴

### 2019/04 - : クラスメソッド株式会社 (現職)

* 職務: SRE

#### Amazon ECS で稼働している Microservice 基盤を Amazon EKS へ移行

* EKS を用いた Kubernetes 基盤への移行作業を担当
* monorepo + kustomize を用いて manifest を管理
* Argo CD を用いた GitOps の実践
  * Secret は [bitnami-labs/sealed-secrets](https://github.com/bitnami-labs/sealed-secrets) を使用して Git に commit
  * 一部の Secret は kubesec + KMS を用いて暗号化している
* 属人化させないためのドキュメントの記述, 開発者を巻き込んでの Kubernetes 説明会/勉強会の開催
* ツール開発
  * [github.com/d-kuro/restart-object](https://github.com/d-kuro/restart-object)
  * [github.com/d-kuro/sealed-secrets-key](https://github.com/d-kuro/sealed-secrets-key)

### 2018/03 - 2019/04 : クラスメソッド株式会社 (現職)

* 職務: ソフトウェアエンジニア

#### EC, CRM 向け API プラットフォーム [prismatix](https://prismatix.jp/) の開発

* AWS 環境における Amazon ECS を使用した Microservices 開発
* Java + Spring Boot を用いた複数の Microservices 開発に従事
  * ポイントサービス
  * 外部 API を用いた決済サービス
  * Elasticsearch を用いた検索サービス
    * Elasticsearch のユーザ辞書, シノニム機能を用いたアプリケーション機能の開発
  * 更新データを Amazon Kinesis から受け取り Elasticsearch に同期するサービス
* Elasticsearch 2.x -> Elasticsearch 6.x 以降に伴うアプリケーションの変更対応
* GitHub の Pull request ベースでのコードレビュー
* CircleCI による CI
* CloudFormation による Infrastructure as Code の実施
* 社内勉強会の企画, 開催
  * Golang もくもく会
  * 技術共有会 (週1開催)
  * Kubernetes 完全ガイド輪読回 (週1開催)

### 2017/04 - 2018/02 : 株式会社テクノモバイル

* 職務: ソフトウェアエンジニア

#### 大手ECサイトの新サービス開発

* 新卒入社
* 同タイミングで入社した社員と異なり研修期間をスキップ
* 実装フェーズからアサイン
* Java + Spring Boot を用いたアプリケーション開発
* GitLab の Merge request ベースでのコードレビュー
* Jenkins による CI/CD
* 結合テスト段階からフロントサーバの管理役として従事
  * フロントサーバ内で発生したバグ対応
  * 要件漏れに伴うお客様説明
  * 要件のすり合わせ等も行う
* バックエンド API の機能追加対応
* 性能試験
  * JMeter を使用
  * AWS 環境下でのインフラ対応
  * アプリケーションのボトルネック検出, 対応
    * リードレプリカ対応
  * シェルスクリプトを用いたログ計測, 解析
* 外部 API を用いた決済システム, 決済を伴う新機能の開発
  * フロントエンド, サーバサイド共に担当
  * 設計, 実装を行う
