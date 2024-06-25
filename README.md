# DependencyTrack-frontend-ja

このプロジェクトは、[Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) の日本語化に関するものです。
オリジナルの en.json を日本語に翻訳しています。

* *注: なお、このプロジェクトは、本家の [Dependency-Track](https://dependencytrack.org/) と関係はありません（個人が趣味的にやっているものです）。*

* *注：v4.11.0 以降、日本語を含む多言語翻訳が公式リリ－スに含まれていますが、一部日本語訳が不自然なため、独自の日本語訳メッセージ ファイルをここで公開しています。*

# 利用方法

1. 利用中の Dependency-Track API サーバーに対応した [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) のソースコード (*1) をダウンロードします。
2. Dependency-Track Frontend のバージョンと一致するバージョンのソース コード (*2) をこのリポジトリからダウンロードします。
3. (*1) を解凍したあとに (*2) を上書き展開します。
4. ターミナルを開き、以下のコマンドを実行します。
```
$ cd /path/to/Dependency-Track-Frontend/
$ npm install
$ npm run build
```
5. コマンド ```npm run build``` の実行が成功したら、```dist/static/config.json``` を適切に編集します（削除でも可）。
6. ```dist/``` 配下のファイル・ディレクトリ群を Dependency-Track Frontend サーバーのドキュメント ルートにコピーします（独自に Docker イメージを作成するのも可）。
7. v4.11.0 未満の場合、Web ブラウザの使用言語の順番で日本語が最優先されるように設定を構成して、Dependency-Track Frontend サーバーにアクセスします。v4.11.0 以降の場合は、ログイン後の右上メニューから日本語を選択します。

![Dependency-Track_Dashboard_ja](https://user-images.githubusercontent.com/100552204/174016314-3b4dfc38-83c4-4b82-8f93-1b5d6dd8697e.png)
