---
layout: page
title: "git-memo"
permalink: /docs/git-memo
---

# ソフトウェア工学 2024

## ソフトウェア工学概論

### ソフトウェアの定義

1, 実行されることによって必要な特性、機能、性能を提供する命令語群（コンピュータプログラム） 

2, プログラムが適切に情報を扱うことを可能とするデータ構造 

3, プログラムの操作や使用法を記述した情報 

### ソフトウェア工学の必要性

1, 大規模化と複雑さ

2, IT人材の不足

3, 社会性と求められるミッション

4, 不確実性の増大

### Hyrumの法則

　あるAPIに十分な数のユーザーがいるとき、APIを作った者自身が契約仕様として何を約束しているかは重要ではない。作られたシステムが持つあらゆる観察可能（observable）な挙動に関して、それに依存するユーザーが出てくるものである。

### スケーラブルなソフトウェア

　変更すべき全てのものを安全に変更可能で、かつコードベースの存続期間を通してそれが可能であるとき、組織のコードベースは持続可能である。

### コストの種類

・財務コスト（例：資金）

・資源コスト（例：CPU時間）

・人件コスト（例：エンジニアリング労力）

・処理コスト（例：行動を取る場合にどんなコストがかかるか)

・機会コスト（例：行動を取らない場合にどんなコストがかかるか）

・社会コスト（例：この選択が社会全般にどのような影響を及ぼすか）

## ソフトウェアライフサイクル

### ソフトウェアライフサイクルとは

1, ソフトウェアの誕生

2, ソフトウェアの開発・運用

3, ソフトウェアの廃止

の順番で行う。

### 要件定義

・実現する機能、実現しない機能を明確にすること

・企業によっては要件定義項目をテンプレート化し、もれなく検討ができる工夫も

#### 要件定義の意義

・プロジェクト関係者のバイブル

・社内外への宣言と協力依頼

・Request for Proposal (RFP)

### 設計

・要件定義書から設計書へ

・コーディングができるレベルの仕様書に落とし込む

・WBS (Work Breakdown Structure)

### 制作

・設計書に従ってシステム構築

・内製（自社開発）

・調達（外部委託）

### オフショア開発

・賃金の安い（安かった）海外企業に外部委託する手法

・注意事項は、文化の違い、言語の違い、商習慣の違い、品質に対する意識の違い

### テストとデバッグ

・バグのないソフトウェアはない（と考えるべき）

・あらかじめテストしバグを早期に発見・対処することが理想

・すべてをテストすることは不可能（工数に限界）

### 運用・保守

・稼働後のデータをプロアクティブに活用するべき

・ソフトウェア以外の要因も考慮する必要がある

・開発者はプロジェクトから離れている可能性がある

### ドキュメンテーション

・複数人でのソフトウェア開発

・非同期コミュニケーションが重要（文書でのコミュニケーション）

・文書は日本語とは限らない

## プロジェクト

### プロジェクトとは

・有期性（必ず終わりがある類の仕事）

・独自性（独自の目的を達成する類の仕事）

### フォアキャスティング・バックキャスティング

#### フォアキャスティング

・インプット視点（どれだけやったか）

・今の立ち位置から順に目標に進んでいく

・目標に到達できない可能性がある

・目標と遠いところに到達する可能性がある

#### バックキャスティング

・アウトプット視点（何を成し遂げたか）

・定めた目標に向けて何が必要かを計画し達成に向かう

・目標を明確に設定する必要がある

・目標に向けての筋道を検討する必要がある

・目標に向けての筋道は適宜修正可能である（事が多い）

・プロジェクト業務はバックキャスティング

## ソフトウェア分析

### ソフトウェアを見える化するための手法

・ソフトウェアの物量に関する分析

・ソフトウェアの実行性能に関する分析

・ソフトウェアのの開発工数に関する分析

・ソフトウェアの品質に関する分析

### QCDの優先度

・品質優先：人命に影響があるようなシステム

・費用優先：公共関連システム

・納期優先：イベント行事関連システム

### ソフトウェアの評価

1, コードの物量（ステップ数）

2, コードの物量（オブジェクト容量）

3, ファンクションポイント（FP）法

4, 使い勝手

#### ファンクションポイント法

プログラミングフェーズに入る前にユーザー要件が定まり、必要な機能が見えてきた段階でシステム規模を概算することができる

・FP値 ＝ 基準値 ×（0.65 + 調整値 / 100）

・原価 ＝ FP値 × 作業単価 × 換算値

## 開発プロセス

### ウォーターフォール型開発プロセス

・進捗管理が容易、成果物が明確

・後工程にしわ寄せが集中というリスクあり

### スパイラルモデル

・プログラム開発を小さなフェーズに分割

・フェーズごとにプロトタイプによるデモンストレーション→フィードバック

・プロトタイプ作成に想定外の作業量が発生するリスクあり

### 反復型開発プロセス

・ソフトウェアを機能分割し、これを「反復」と呼ぶ単位で管理する。

メリット

・・部分的に完成させていくので、顧客の要求を取り入れやすい

・・部分的な納品が可能

デメリット

・・分割のための作業や管理業務が増える

・・全体像が見えづらい

・・一括して稼働するシステムは分割しても意味がなくなってしまう

### アジャイルプロセス

・変化に対応して無駄を廃し、最適な手法で動くソフトウェアの提供を優先する

・ウォーターフォール型開発プロセスでは想定されていなかった「できるだけ決定を遅らせる」、「できるだけ早く提供する」を実現

・モチベーションを上げ、学習効果を高めることで無駄をなくす

#### アジャイルの価値

・プロセスやツールよりも、個人や個人や相互作用

・わかりやすいドキュメントよりも、動くソフトウェア

・契約上の駆け引きよりも、顧客とのコラボレーション

・計画を硬直的に守るよりも、変化への対応

#### アジャイルのコンセプト

・変化の受容性、速いサイクル/頻繁な納品、シンプルな設計、リファクタリング、レトロスペクティブ、暗黙知、テスト駆動型開発

#### アジャイル開発の12の原則

1, ソフトウェアの早期、継続的な納品によって顧客の満足度を達することが最優先である。

2, 開発の終盤であろうとも、要求内容の変更を欲迎する。アジャイルなプロセスは、顧客の競争上の優位性のため、変化を制する。

3, 数週間から数か月のサイクルでソフトウェアを納品する、サイクルは短いほうがよい。

4, ビジネス側の人間と開発者がプロジェクトを通じて日々協力しなければならない。

5, 志の高い開発者を中心にプロジェクトを編成する。必要な環境や支援を与え、任務をやり遂げることを信じること。

6, 開発チームの内外で最も効率的で効果的な情報伝達を行う手段は、顔を突き合わせることである。

7, 動作するソフトゥェアが主たる進捗の確認手段である。

8, アジャイルなソフトウェア開発は、持続的な開発を促す。開発資金の提供者、開発者、ユーザは、必ず一定のペースを守るべきである。

9, 技術力とよい設計に絶えず気を配ることで、機敏さを向上する。

10, 不必要なことは行わないという簡潔さは本質的である。

11, 自己組織化されたチームから最新のアーキテクチャ、要求、設計が生まれる。

12, 定期的に、チームはもっと効果的になる道を考え、開発の進め方を調和させ、調整する。

### リスク駆動型開発プロセス

想定されるリスクをあらかじめ把握する

・アジャイル

・計画駆動形

・アジャイル/計画駆動形共通

・予測不可能なリスク

### WBS（Work Breakdown Structure）

プロジェクト目標を達成し、必要な要素成果物を生成するために、プロジェクトチームが実行する作業を、要素成果物を主体に階層的に要素分解したもの

・プロジェクトを細かな作業（Work）に分解（Breakdown）した 構成図（Structure）

・作業を細かく分解し（これが難しい）、作業順に並べる

#### WBSの作り方

・スコープを明確にする

・大きな作業をグルーピングする

・グループングした作業の相互関連を考える

・各グループの作業を洗い出す

## UML

### UMLとは

・万国共通の記法

・オブジェクト指向プログラミング

・文章によるドキュメントに加えて開発・設計を図示化（モデル化）する

・論理ビュー（クラス図、オブジェクト図など）

・プロセスビュー（アクティビティ図など）

・開発ビュー（パッケージ図、コンポーネント図など）

・物理ビュー（配置図など）

・ユースケースビュー（ユースケース図など）

#### ユースケース図

・アクター

・ユースケース

・関連

・システム境界

#### アクティビティ図

・システム内部で行われていることを表現する

・各ユースケースをどのようなプロセスで実現するかを記載

・アクションノード：角が丸い長方形

・矢印

・初期ノード

・最終ノード

・フォーク

・ジョイン

#### クラス図

・オブジェクト指向モデル

・クラス

・オブジェクト

・インスタンス

・属性

・操作

#### オブジェクト図

・クラスに中身を入れた状態のもの

・クラス図を作成するための中間生成物的な位置づけ

#### シークエンス図

・時間の前後関係やタイミングを表現できる

#### コミュニケーション図

・シークエンス図を書き換えたもの

・通信リンクを使って接続形態やネットワーク構成が表現できる

#### タイミング図

・オブジェクト間の相互作用のタイミングと状態遷移を表現したもの

#### 相互作用概要図(iod)

・システムの鳥瞰図

・sd: シークエンス図

・cd: コミュニケーション図

・td: タイミング図

・これらの相互作用をアクションとするアクティビティ図

#### コンポーネント図

・コンポーネント：複数のクラスで構成される処理に対して１つ以上のインターフェースを用意し、あたかも１つのクラスのように取り扱ったもの

・カプセル化されたソフトウェアパーツの管理を目的とした図

・「コンポーネント」はタグ付アイコンで表現

・要求インターフェース

・提供インターフェース

#### パッケージ図

・クラス図のうち”package”であるクラスを抽出

・パッケージの依存関係を表現し管理

#### 状態マシン図

・トリガーによるオブジェクトの状態遷移を表現

#### 配置図

・ハードウェアの構成を表現

## コーディング

### コーディングとは

・コードは書くよりも読まれることの方が多い（Python コードのスタイルガイド）

・ソフトウェア開発にあたり読みやすいコードを書くことは必須

### コードのレイアウト

・79文字以内にする。docstring やコメントは72文字以内にする。

・行を継続する場合は、折り返された要素を縦に揃える（Hanging indentation）

・1レベルインデントするごとに、スペース（タブではなく）を4つ使う

### スペース

・演算子の前後にスペースを前後に一つずつ空ける

・無駄なスペースを入れない

### 改行

・文を重ねない

・演算子の位置を揃える

### import

1, 標準ライブラリ

2, サードパーティに関連するもの

3, ローカルなアプリケーション/ライブラリに特有のもの

### その他

・UTF-8以外のエンコーディングは可能な限り使わない

・ASCII文字以外の使用を極力避ける

・PEP8のスタイルガイドに合わせることは重要だが、プロジェクトの中で一貫性を保つことはもっと重要

## バージョン管理

### バージョン管理とは

・ファイルを「誰が」、「いつ」、「どのように」変更したかを管理する

・これらの情報が管理されていれば、多数のメンバーとも共同でコード開発ができる

・集中管理型

・分散管理型

#### 集中管理型

・同時編集するとコンフリクトが発生しやすい

・同期に時間がかかる

#### 分散管理型

・リモートリポジトリへのアクセス頻度が低い

・障害に頑健

## git

### gitとは

・分散管理型のバージョン管理システム

・元々はオープンソースソフトウェア管理のためのソフトウェア

・変更履歴が残る

・変更した箇所に戻ることができる

・他人と共同編集できる

### コミット

・ファイル作成／変更／削除の記録

・対象ファイルは一つでも複数でもよい

・コミットの単位はユーザーが自由に決定する

### レポジトリ

gitが管理するプロジェクトのフォルダ

・ローカルレポジトリ

・リモートレポジトリ

#### ローカルレポジトリでの流れ

##### ワークツリー

・untracked（gitで管理されていないファイルの状態）

・unmodified（gitで管理されているが変更されていないファイルの状態）

・modified（gitで管理されていて変更されたファイルの状態）

##### ステージングエリア、インデックス

・gitで管理するファイルを登録する

・staged（staging areaに登録されたファイルの状態）

##### Gitディレクトリ

・コミット(commit)により変更を登録

・commitは原則、変更・削除できない

・commitされたファイルはunmodifiedの状態になる

#### リモートレポジトリの流れ

・ローカルレポジトリでcommitされた変更をリモートレポジトリへ反映(git push)

・リモートレポジトリにある内容をローカルレポジトリに反映 (git pull)

### ブランチ

・作業を枝分かれさせることができる（共同作業・並行作業が可能）

### .gitignore

・gitに管理してほしくないファイルを指定する

## gitコマンド

### 設定・確認系

・git init（gitの初期化・設定開始）

・git status（ワークツリーのステータスを表示）

・git config（設定周りの確認・変更）

・git log（ログを表示）

・git diff（ファイルの差分を表示）

### コミット系

・git add（ステージングエリアに追加）

・git commit（コミットの実行）

### 修正系

・git commit --amend --no-edit（コミットの修正）

・git checkout（削除されたファイルを復旧や過去コミットの復元など（元に戻す変更がstaging area/index内にある場合））

・git reset（コミットのリセット）

・git revert（「コミットの変更を打ち消す」コミット）

・git rm（ファイルとindex情報の削除）

### リモート系

・git clone（レポジトリをコピー）

・git pull（リモートレポジトリの同期）

・git push（変更をアップロードする）

・git request-pull（プルリクエスト：変更依頼）

・git remote（リモートレポジトリの設定）

### ブランチ系

・git branch（ブランチの作成）

・git checkout（ブランチの切り替え）

・git merge（ブランチの統合）

・git clone（レポジトリをコピー）

・git push（変更をアップロードする）

## github

### githubとは

・リモートレポジトリのホスティングサービスの一つ

・オープンソースソフトウェアの主要なポータルサイト

### Githubでのソフトウェア・エンジニアリング

・clone/fork

・template（いくつでもforkできる）

・issues（レポジトリに関する問題・課題・バグ・機能追加や質問などを挙げるための機能）

・projects（issuesなどを管理するためのテーブル・kanban）

## CI/CD

### Continuous Integration（CI）

・コード変更を共有リポジトリに頻繁に統合するプロセス

・自動テストとビルドを定期的に実行し、バグの早期発見と修正を可能に

・CIの自動化により開発のスムーズな進行を促進

### Continuous Delivery（CD）

・コード変更をテスト環境や本番環境に自動的にデプロイするプロセス

・自動デプロイメントを組み込み、手動操作によるデプロイの必要性を排除

・CDにより、ユーザーフィードバックを迅速に反映可能

### CI/CDパイプラインの基本的なステップ

1, ソース: コード変更をトリガーにワークフローを起動

2, ビルド: ソースコードをコンパイル

3, テスト: 自動テストを実行

4, デプロイ: テスト済みのコードを本番環境にデプロイ

5, 検証: デプロイされたアプリケーションの動作確認

6, モニタリング: 本番環境での継続的な監視

### GitHub Actionsを使用したCI/CD

1, ワークフローの定義: YAMLファイルで定義し、 .github/workflows/ディレクトリに配置. イベント、ジョブ、ステップで構成

2, トリガー:  プッシュ、プルリクエスト、スケジュールなど様々なイベントでワークフローを起動可能

3, ジョブとステップ: ジョブは並列実行が可能. ステップでは、シェルコマンドの実行やアクションの使用が可能

4, アクション: 再利用可能なワークフローの構成要素. コミュニティが作成したアクションも利用可能

5, ランナー:  GitHub提供のホステッドランナーまたはセルフホステッドランナーを使用可能

## CI/CDの実践（Github pages）

### Github Pages

・Githubにあるリモートレポジトリの内容をwebpageとして公開することができる

・HP更改はCI/CDにより自動化

・Jekyllを使用することでmarkdownファイルを自動でhtml化することができる（開発者はmarkdownファイルを作成すれば良い）

## テスト手法

### テストコード

・バグの早期発見のために手間をかける

・本分析とは別にテストコードを用意する

### ソフトウェアのテスト

・ブラックボックステスト（内部処理をブラックボックス（何をやってるかわからない）として対処）

・ホワイトボックステスト（中身を見ながら行うテスト）

### テストの範囲

・テストデザイン

・やみくもにテストすると手間がかかる

### テストの自動化

・ソフトウェアの迅速な開発へ

・ヒューマンエラー防止

・テストの効率化

・ツールを活用

・継続的インテグレーション（CI）

## デバッグ

### デバッグ（debug）

・バグを取り除く作業

・リアクティブアプローチ

・プロアクティブアプローチ

### PDCA（Plan Do Check Action）

・Plan（目標・目的を設定し、実行計画を立案）

・Do（計画の実行）

・Check（実行内容の検証）

・Action（検証結果からの改善点の検討）

## 卒業研究

### 卒業研究の特徴

#### 卒業研究をソフトウェア開発と捉えてみる

##### 成果物

・卒業論文

・実装、分析コード

##### 参画人数

・一人もしくは少数（院生・教員ともに）

##### 内容

・テーマ選定

・関連研究調査

・実装、分析

・結果の考察

### 卒業研究のためのバックキャスティング

・研究目的を明確に設定する必要がある

・研究目的は具体的かつ達成する価値のあるものにする（イシュー）

・研究目的は適宜修正可能である

・研究目的に向けての筋道は適宜修正可能である（事が多い）

・研究活動はバックキャスティング