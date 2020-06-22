# Resume

* [GitHub Pages link](https://d-kuro.github.io/resume/)

## Personal Information

| key  | value |
| - | - |
| Name | Dai Kurosawa |
| Sex | 男 |
| Age | 25 |
| Mail | [kurosawa7620@gmail.com](mailto:kurosawa7620@gmail.com) |
| Twitter | [@ponde_m](https://twitter.com/ponde_m) |
| GitHub | [@d-kuro](https://github.com/d-kuro) |
| Blog 1 | https://d-kuro.github.io/ |
| Blog 2 | https://ponde-m.hatenablog.com/ |

## Introduction

現職は Quipper という会社で SRE をやっています。
プロダクションにて Kubernetes クラスタが動作しているのでその運用/改善などや CI/CD 基盤の構築/改善などの仕事をしています。

Kubernetes については関心が強く、趣味/仕事でソースコードを読んでいたりで細かい仕様に対する理解があります。過去には Kubernetes Meetup Tokyo などで LT をしたりしました。

* https://speakerdeck.com/daikurosawa/introduction-to-descheduler
* https://speakerdeck.com/daikurosawa/argo-cd-practice-guide
* https://speakerdeck.com/daikurosawa/leader-election-in-kubernetes-number-k8sjp

Kubernetes の上で動作させるアプリケーションについてどのようにするべきか、などの心得もあり、開発者への周知や Prodction Readiness Check などでのレビューなどを行っていたりします。

SRE として働く前はソフトウェアエンジニアとして働いており、バックエンドのマイクロサービスの開発を行っていたため、バックエンドエンジニアとしての経験もあります。

プログラミング言語は Go が得意で Go のお作法にしっかり乗っ取りつつ、パフォーマンス等を意識してコードを書くことができます。
コマンドラインツールから API の設計/開発まで一通りの心得があります。
最近では趣味仕事を通して最近は基本的に Go を書いていますが、Java/Spring Boot の経験もあります。

個人では初学者向けに Go のメンターなどをやっていたりします。

https://menta.work/plan/1348

GitHub: https://github.com/d-kuro
Twitter: https://twitter.com/ponde_m

## Skill

### Go

* Go のお作法にしっかり乗っ取りつつ, パフォーマンス等を意識してコードを書くことができる
* API や CLI ツールを作成することができる
* goroutine や channel を利用し, Go らしい並行処理を書くことができる

### Kubernetes

* 業務では Kubernetes Cluster をプロダクションで運用中
* Argo CD を用いた GitOps など, 周辺のエコシステムに関してもキャッチアップを行なっている
* kubectl を用いた操作や Manifest の記述を行うことができ, Kubernetes の基本的なアーキテクチャについて理解している
* 必要に応じて Kubernetes 本体やエコシステムのソースコードから読み込みを行うことができる
  * [Kubernetes で Deployment のローリングアップデートを実現する kubectl rollout restart コマンド解説 - あふん](https://ponde-m.hatenablog.com/entry/2019/06/18/010332)
  * [Kubernetes のソースコードとの付き合い方 #gounco / Kubernetes source code reading](https://speakerdeck.com/daikurosawa/kubernetes-source-code-reading)
  * [Kubernetes Leader Election in Depth - AFN Blog](https://d-kuro.github.io/posts/kubernetes-leader-election/)
* clinet-go を用いた小さめのアプリケーションを開発を経験

### Java

* Spring Boot を用いたアプリケーションの開発を2年程度経験
* API を開発することができる

### 英語

* 英語で書かれた文書を翻訳を使いつつ、理解することができる

## 興味 & 関心

* SaaS 開発
* Kubernetes を用いた Microservice 環境化 SRE として組織生産性を高めるための仕組みづくりをしていきたい
  * Microservice という複雑な環境下で Microservice のチーム単位でオーナシップを持ち Dev から Ops まで回していけるような仕組みづくり 
* プログラミング言語は Go を使いたい
  * 一番得意なプログラミング言語
  * シングルバイナリになることからのツール開発等での相性の良さ
  * Kubernetes, Docker 等のコンテナ界隈での採用率

## 職務経歴

### 2019/10 - : Quipper, Ltd  (現職)

* 職務: SRE

#### Kubernetes プラットフォームの開発構築

* kube-aws で構築されている Kubernetes クラスタの構築/アップグレード
* monorepo 環境における GitOps を用いた CD 基盤構築
* システムコンポーネントや kustomize 等のツール類のアップグレード
* 監視設定の見直し
* アプリケーションのリソースチューニング
* HPA の導入
* manifest のポリシーを記載し開発者に周知
* 開発者への Kubernetes 周辺技術のサポート

#### その他 SRE 業務

* 既存の CI/CD 環境の改善
* アラート対応
* 新規サービス開発時の Design Doc レビュー
* Production Readiness Check

### 2019/04 - 2019/09: クラスメソッド株式会社

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

### 2018/03 - 2019/04 : クラスメソッド株式会社

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

## 労働環境に関する希望

> 📝
>
> 現在は副業を探しており週 8 ~ 16 時間程度の間でフルリモートにて働ける会社を探しています。
> 
> * Go を用いたバックエンドの API 開発
> * Kubernetes などを導入している企業での運用サポート/アドバイス/トラブルシューティング
> 
> などを得意としているためそこら辺に携わることができるお仕事だと強みを発揮できるかなと思っています。

* 技術力向上がしやすい環境
  * 技術力向上に対する意欲の高い人が多い
  * モダンな技術に挑戦できる
  * 勉強会, 企業ブログ等で外部へのアウトプットを行なっている
  * 業務時間内でのカンファレンス参加等が認められている
  * 書籍購入費, カンファレンス参加費, 資格試験費などがある程度補助される
* フレックス制度
  * ある程度自分の裁量で就業時間をコントロールでき, 勉強会などに参加しやすい環境

## 資格

* 2018/06/27
  * AWS Certified SysOps Administrator - Associate Level
* 2018/06/18
  * AWS Certified Developer - Associate Level
* 2018/05/30
  * AWS Certified Solutions Architect - Associate Level
* 2016/12
  * ネットワークスペシャリスト試験
* 2016/06
  * データベーススペシャリスト試験
* 2015/06
  * 情報セキュリティスペシャリスト試験
* 2014/12
  * 応用情報技術者試験
* 2013/11
  * 基本情報技術者試験
* 2012/11
  * ITパスポート試験

## Speaker

* 20200613
  * [KubeFest Tokyo 2020](https://k8sjp.github.io/kubefest-2020/)
  * [Understanding CPU throttling in Kubernetes to improve application performance #k8sjp - Speaker Deck](https://speakerdeck.com/daikurosawa/understanding-cpu-throttling-in-kubernetes-to-improve-application-performance-number-k8sjp)
* 20200129
  * [Kubernetes Meetup Tokyo #27 - connpass](https://k8sjp.connpass.com/event/162343/)
  * [Leader Election in Kubernetes #k8sjp - Speaker Deck](https://speakerdeck.com/daikurosawa/leader-election-in-kubernetes-number-k8sjp)
* 20190726
  * [Kubernetes Meetup Tokyo #21 - Cloud Native CI/CD - connpass](https://k8sjp.connpass.com/event/138375/)
  * [Argo CD 実践ガイド #k8sjp / Argo CD Practice Guide](https://speakerdeck.com/daikurosawa/argo-cd-practice-guide)
* 20190531
  * [Kubernetes Meetup Tokyo 19 (Yahoo! JAPAN MEETUP共催)](https://k8sjp.connpass.com/event/126207/)
  * [図で理解する Descheduler #k8sjp #ymju / Introduction to Descheduler](https://speakerdeck.com/daikurosawa/introduction-to-descheduler)
* 20190527
  * [Go(Un)Conference（Goあんこ）LT大会 6kg](https://gounconference.connpass.com/event/129090/)
  * [Kubernetes のソースコードとの付き合い方 #gounco / Kubernetes source code reading](https://speakerdeck.com/daikurosawa/kubernetes-source-code-reading)
* 20180131
  * [Go(Un)Conference（Goあんこ）LT大会 5kg](https://gounconference.connpass.com/event/112942/)
  * [GolangCI を使ってコードの品質を保ちながら快適な Golang 生活を送る話 #gounco / GolangCI - Speaker Deck](https://speakerdeck.com/daikurosawa/golangci)
* 20181214
  * [Introduction gRPC](https://speakerdeck.com/daikurosawa/introduction-grpc)
* 20180918
  * [Gopher道場#3 卒業式＆LT大会](https://mercari.connpass.com/event/101178/)
  * [Go Cloud を触ってみる / gopher-dojo-lt](https://speakerdeck.com/daikurosawa/gopher-dojo-lt)
