# コマンドメモ
## VSCODE
- VSCODEでターミナル起動
    - control + shift　+　`
- 置換
    - option + command + f
- 複数行まとめて処理
    - option + command + カーソル

## git
- ローカルリポジトリの初期化
    - git init
- インデックスにファイルを追加（更新対象インデックスにファイルを追加する。　-A は全て選択。）
    - git add -A
- 変更を反映（コミット）
    - git commit -m "コメント"
- githubで新規リポジトリ作成
    - https://qiita.com/sodaihirai/items/caf8d39d314fa53db4db
- githubのリモートリポジトリ情報をローカルリポジトリに追加
    - git remote add origin [リモートリポジトリのURL]
- ローカルリポジトリの変更をリモートリポジトリに反映
    - git push origin master

## その他便利コマンド
- jsonをcsvに変換したい。
    - csvkitのインストール
        - pip install csvkit
    - 変換
        - in2csv saenai.json -k record -f json > saenai.csv
        -kでKeyを指定、-fでファイルを指定。リダイレクトでCSVファイルに出力。

# お勉強参考URL
- Auth0をReact＋Expressのアプリケーションで実装する（公式ブログ）
　　- https://auth0.com/blog/jp-react-tutorial-building-and-securing-your-first-app/#React----------------------------------
