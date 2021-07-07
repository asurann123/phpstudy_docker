# phpstudy_docker
- phpの勉強環境をdockerにて構築
- PHP(PDO含),MySQL,phpMyAdmin環境を一発で構築
---

## セットアップ
1. mkdir {appropriate directory name}
2. git clone {this repository url} .  
→ . を付けておくことでgit cloneしたときにphpstudy_dockerというディレクトリが作成されないようになる
3. docker compose up -d
4. Complete!!!

---

## 仕様等
1. PHP
   * http://localhost:5050/
   * src配下のファイルが対象  
      -> src/practice/manu.phpの場合[http://localhost:5050/practice/php/menu.php]にアクセスする  
     
2. phpMyAdmin  
   * rootアカウントでログインされているので、基本的には何でもし放題??🥺

---

## docker-composeやDockerFileを変更した場合
PHPやMySQLのバージョンを変更した場合等  
1. 動いているDockerコンテナを停止
2. Dockerコンテナを削除
3. docker compose buildを実施
4. docker compose up -d
5. OK!!!!!!!
