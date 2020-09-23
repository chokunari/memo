# コマンドメモ
## ローカル
- docker commit コンテナID リポジトリ名:タグ
    - `docker commit 10c309d97383 chokunari/diveworksfront:v_0.2`
- docker push リポジトリ名:タグ
    - `docker push chokunari/diveworksfront:v_0.2`

## cloud shell
- dockerイメージ取得
    - `docker pull chokunari/diveworksfront:v_0.2`
- タグづけ
    - `docker tag chokunari/diveworksfront:v_0.2 asia.gcr.io/nttd-platformtec/cn-horitan-app01-front:front-v_0.2`
- dockerイメージをpush
    - `docker push asia.gcr.io/nttd-platformtec/cn-horitan-app01-front`
- マニフェスト適用
    - `kubectl apply -f manifest_deploy.yaml`
- pod確認
    - `kubectl get pods`
- podのログ確認
    - `kubectl describe pods cn-horitan-app01-front-pod-687b4fd6c5-wwtfv`
- podのログ詳細確認
    - `kubectl logs cn-horitan-app01-front-pod-687b4fd6c5-wwtfv`

## その他便利コマンド
- プロセス確認
    - `ps aux | grep hogehoge`
- プロセスキル
    - `kill プロセスID`
- grep
    - `rep -lr hogehoge --include="*.html" /var/www/htm`
