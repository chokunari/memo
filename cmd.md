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
### 困った時は
    - remote containerで前のパスを見に行くためコンテナにリモートできてなさそう・・・？
        - ファイル→開く→存在するパスを指定すれば開ける。

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
- Docker network作成
    - `docker network create wtgnet`

## GCP
- GCP SDKインストール
    - https://cloud.google.com/sdk/docs/quickstart-macos?hl=ja
- storageへアップロード
    - `gsutil cp $HOME/local_folder/file1.png gs://bucket-ca4/`

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

## CSS
- position
    - https://www.legit.co.jp/position/10685
    - http://www.htmq.com/style/position.shtml
    

# お勉強参考URL
- Auth0をReact＋Expressのアプリケーションで実装する（公式ブログ）
    - https://auth0.com/blog/jp-react-tutorial-building-and-securing-your-first-app/#React----------------------------------

- API一覧
    - APIbank
        - https://www.apibank.jp/ApiBank/api?category_no=0
    - public-apis
        - https://github.com/public-apis/public-apis

- アニメ関連のAPI
    - trace.moe
        - アニメ画像をアップロードすると、アニメ動画を検索しマッチしたアニメの情報（タイトルとか）を表示する。
        - https://trace.moe/
    - ShangriLa Anime API Server
        - https://github.com/Project-ShangriLa/sora-playframework-scala

- アニメ関連サービス
    - アニリスト
        - https://anilist.co/