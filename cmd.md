# コマンドメモ
## VSCODE
- VSCODEでターミナル起動
    - ``control + shift　+　` ``
- 置換
    - `option + command + f`
- 複数行まとめて処理
    - `option + command + カーソル`
- コード自動整形
    - `範囲指定後　command + k →　command + f`

## git
- ローカルリポジトリの初期化
    - `git init`
- インデックスにファイルを追加（更新対象インデックスにファイルを追加する。　-A は全て選択。）
    - `git add -A`
- 変更を反映（コミット）
    - `git commit -m "コメント"`
- githubで新規リポジトリ作成
    - https://qiita.com/sodaihirai/items/caf8d39d314fa53db4db
- githubのリモートリポジトリ情報をローカルリポジトリに追加
    - `git remote add origin [リモートリポジトリのURL]`
- ローカルリポジトリの変更をリモートリポジトリに反映
    - `git push origin master`

## Docker
- Docker image作成
    - docker commit コンテナID リポジトリ名:タグ
    - `docker commit 10c309d97383 chokunari/diveworks-front:v_0.2`

- Docker imageをDockerHubにアップロード
    - docker push リポジトリ名:タグ
    - `docker push chokunari/diveworks-front:v_0.2`

## GCP
- GCP SDKインストール
    - https://cloud.google.com/sdk/docs/quickstart-macos?hl=ja

## その他便利コマンド
- jsonをcsvに変換したい。
    - csvkitのインストール
        - `pip install csvkit`
    - 変換
        - `in2csv saenai.json -k record -f json > saenai.csv`
        -kでKeyを指定、-fでファイルを指定。リダイレクトでCSVファイルに出力。
- プロセス確認
    - `ps aux | grep hogehoge`
- プロセスキル
    - `kill プロセスID`
- grep
    - `rep -lr hogehoge --include="*.html" /var/www/htm`

# お勉強参考URL
- Auth0をReact＋Expressのアプリケーションで実装する（公式ブログ）
　　- https://auth0.com/blog/jp-react-tutorial-building-and-securing-your-first-app/#React----------------------------------
