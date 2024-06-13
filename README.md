# DependencyTrack-frontend-ja

This project is a Japanese translation effort of [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend).
Basically, "en.json", which is provided by Dependency-Track Frontend, is translated into Japanese as a file "ja.json",
and some files are modified in order to switch locales.

*NOTE: This project has nothing to do with the original [Dependency-Track](https://dependencytrack.org/).*

*NOTE: As of v4.11.0, Japanese translation is included in the official release, but some of the translated messages are not correct or unfamiliar to the native Japanese people. So, this project is trying to mitigate the translation errors by publishing the custom translation files sseparately.*

《このプロジェクトは、[Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) の日本語化に関するものです。
オリジナルの en.json を日本語に翻訳しており、表示言語を切り替えるための変更を一部のファイルに実施しています。》

*《注: なお、このプロジェクトは、本家の [Dependency-Track](https://dependencytrack.org/) と関係はありません（個人が趣味的にやっているものです）。》*

*《注：v4.11.0 以降、日本語を含む多言語翻訳が公式リリ－スに含まれていますが、一部日本語訳が不自然なため、独自の日本語訳メッセージ ファイルをここで公開しています。》*

# How To Use　《利用方法》

1. Download a source code of [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) (*1) which is compatible with Dependency-Track API server you are using.　《利用中の Dependency-Track API サーバーに対応した [Dependency-Track Frontend](https://github.com/DependencyTrack/frontend) のソースコード (*1) をダウンロードします。》
2. Download a source code on this repository (*2) the version of which matches that of Dependency-Track Frontend.　《Dependency-Track Frontend のバージョンと一致するバージョンのソース コード (*2) をこのリポジトリからダウンロードします。》
3. Unzip (*1), then unzip (*2) with overwriting (*1).　《(*1) を解凍したあとに (*2) を上書き展開します。》
4. Open a terminal and type the following commands.　《ターミナルを開き、以下のコマンドを実行します。》
```
$ cd /path/to/Dependency-Track Frontend/
$ npm install
$ npm run build
```
5. If the command ```npm run build``` is successful, then edit properly a file ```dist/static/config.json``` (, or delete it).　《コマンド ```npm run build``` の実行が成功したら、```dist/static/config.json``` を適切に編集します（削除でも可）。》
6. Copy the files and directories under ```dist/``` to the document root of Dependency-Track Frontend server (, or build your custom Docker image).　《```dist/``` 配下のファイル・ディレクトリ群を Dependency-Track Frontend サーバーのドキュメント ルートにコピーします（独自に Docker イメージを作成するのも可）。》
7. Before v4.11.0, set your browser's preffered language to Japanese, and access Dependency-Track Frontend server.　For versions 4.11.0 or later, sign in and change your language to Japanese on the right-top menu.《v4.11.0 未満の場合、Web ブラウザの使用言語の順番で日本語が最優先されるように設定を構成して、Dependency-Track Frontend サーバーにアクセスします。v4.11.0 以降の場合は、ログイン後の右上メニューから日本語を選択します。》

![Dependency-Track_Dashboard_ja](https://user-images.githubusercontent.com/100552204/174016314-3b4dfc38-83c4-4b82-8f93-1b5d6dd8697e.png)
