# コマンドメモ
## ローカル
- docker commit コンテナID リポジトリ名:タグ
    - `docker commit 10c309d97383 chokunari/diveworksfront:v_0.2`
- docker push リポジトリ名:タグ
    - `docker push chokunari/diveworksfront:v_0.2`

## cloud shell
- dockerイメージ取得
    - `docker pull chokunari/diveworksfront:v_0.2`

## その他便利コマンド
- プロセス確認
    - `ps aux | grep hogehoge`
- プロセスキル
    - `kill プロセスID`
- grep
    - `rep -lr hogehoge --include="*.html" /var/www/htm`
