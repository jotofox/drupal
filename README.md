# Drupalについて

Drupal は個人のブログからコミュニティ駆動の巨大サイトまで様々なウェブサイトをサポートするCMSです。  
より詳しい情報はDrupalの[公式サイト](https://www.drupal.org)をご覧ください。  
また、Drupalのコミュニティへの参加は[こちら](https://ww.drupal.org/community)。  
  
## Drupalの法的情報に関して：
* Drupal利用時の権利にについては`core` ディレクトリ配下の`LICENSE.txt`をご覧ください
* Drupalのトレードマークやロゴについてのポリシーは[こちら](https://www.drupal.com/trademark)をご覧ください

# 設定と機能

*Drupal コア*`drupwl-x.y.tar.gz`もしくは`drupal-x.y.zip`[ファイル](https://www.drupal.org/project/drupal)
には、ウェブサイトを始めるために必要なものが入っています。  
そこには一般的なサイトに必要な、コンテンツの編集、ユーザーアカウント、画像アップロードや検索機能といった、幾つかモジュール（機能を拡張する追加機能）が含まれています。  
コアはサイト特有の設定を許可するオプションを備えています。  
コアモジュールに加えて、ダウンロード可能な（Drupalコアに含まれていない機能を追加するための）外部モージュールがあります。  

## 設定について詳しくは：
* Drupalのインストール、更新、メンテナンスについては、`core`ディレクトリ配下にある`Install.txt`, `UPDATE.txt`をご覧ください。
* [サイトを構築するにあたってDrupalの使い方について](https://www.drupal.org/documentation)
* [ベストプラクティス](https://www.drupal.org/best-practices)
* Drupalの機能を拡張するための`/modules`配下への外部モジュールを[ダウンロード](https://www.drupal.org/project/modules)
* 自身のモジュールを作るために下記の"Drupalの開発"節もご覧ください。

# インストールプロファイル

インストールプロファイルは、モジュールの有効化やContent-Typeの定義等、追加のインストール手順を定義するもので、Drupalを最初にインストールしたとき、ベースとなるインストール処理の後、コアによって作られます。  
このとき、二つのインストールプロファイルがコアによって作られます。  
サイト固有のユースケースに向けて、Drupalコミュティがインストール工程を編集したインストールプロファイル（メディアパブリッシャのためのCMS、ウェブプロジェクトのトラッキングツールや非営利団体の顧客管理システム等）は金策や寄付よって提供されています。  
それらはベアインストールプロファイルやディストリビューションとして配布されています。  
ディストリビューションには、Drupalコアやインストールプロファイルに加えて、カスタムモジュールやテーマ、サードバーティ製のライブラリなどの必要な拡張機能の全てを含んでいます。
ベアインストールプロファイルには、Drupalコアと必要な拡張機能を別々にダウンロードして、インストールを始める前の`/profiles`ディレクトリにダウンロードしたプロファイルを配置します。

## インストールプロファイルとディストリビューションについて詳しくは：
* [インストールプロファイルとディストリビューションの違いについて](https://www.drupal.org/node/1089736)
* [ダウンロードはこちら](https://www.drupal.org/project/distributions)
* [カスタムインストレーションプロファイルとディストリビューションの開発について](https://www.drupal.org/docs/8/creating-distributions)

# 外観

Drupalにおいて、サイトの外観はテーマによって設定されます。（テーマはフォント設定や色、レイアウトなどの拡張です）  
Drupalコアにはいくつかのテーマが入ってます。  
さらにダウンロードできるテーマがあり、自身のカスタムテーマを作ることもできます。  

## テーマについて詳しくは：
* Drupalの外観を変更するための`/themes`ディレクトリに入れる外部テーマの[ダウンロード](https://www.drupal.org/project/themes)
* [自身のカスタムテーマの開発について](https://www.drupal.org/docs/8/theming)

# Drupal の開発

Drupalにはサイトの機能を変更したり追加するために許可された拡張APIがあります。  
APIは`hooks（フック）`で構成されており、システムイベントに反応し、Drupalの動作をカスタマイズし、データベースクエリやフォーム生成などの一般的な操作を標準化します。  
柔軟なフックというアーキテクチャは、Drupalコアにあるファイルを直接編集しなくても望む機能を獲得できるということを意味します。  
また、機能の変更はモジュールの形式を取っています。  
Drupalサイトに新しい機能を追加したい時、既存の外部モジュールを検索してください。  
もしモジュールを見つけてもバグや必要な追加機能がなければ、モジュールを修正し`patch（パッチ）`の形式でプロジェクトの改善に貢献してください。  
欲しい機能に近いものが存在しない場合にだけ、新しいカスタムモジュールを作成してください。

## 開発について：
* [外部モジュールの検索](https://www.drupal.org/project/modules)
* [パッチへの貢献](https://www.drupal.org/patch/submit)
* [モジュール開発について](https://www.drupal.org/developing/modules)
* [従うべきプログラミングのベストプラクティス](https://www.drupal.org/developing/best-practices)
* [APIドキュメンテーション](https://www.drupal.org/api/drupal/8)
* [Drupal API の例示ドキュメントから学ぶ](https://www.drupal.org/project/examples)

# 詳細情報
* [Drupal.org のオンラインドキュメンテーション](https://www.drupal.org/documentation)
* セキュリティについてのアナウンス一覧は、["Security advisories"ページ](https://www.drupal.org/security)をご覧ください。（RSSフィードとして有効）<br>このページではEメールでアナウンスを購読する方法も説明されています。
* Drupalのセキュリティプロセスについての情報、Drupalのセキュリティチームに潜在的なセキュリティ問題を報告する方法については、["Security team"ページ](https://www.drupal.org/security-team)をご覧ください。
* さまざまなサポートオプションについては、[こちら](https://www.drupal.org)にアクセスし、上部または下部のナビゲーションで`Community and Support`をクリックしてください。
