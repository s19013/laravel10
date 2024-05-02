# 
laravel + mysql + nginxの基礎キットです｡  
※ 個人用故保証できません｡  

laravel10

# 手順
1. `.env.example`を同じディレクトリ内でコピー
2. コピーしたファイルの名前を`.env`に変更
3. vscodeとかのターミナルで`docker compose -d`

db,pmaの環境変数はlaravelの.envファイルを参考することにした｡  
余計なものも含まれるが動作に影響はないため機にしない｡

## desktop を使う場合
4. backend-containerのexecタブで`compose install`
5. 続けて､`php artisan key:generate`


## コマンドラインを使う場合
4. `docker compose exec backend-containe composer install`
5. `docker compose exec backend-containe php artisan key:generate`
6. `php artisan serve --host 0.0.0.0`

# 参考にしたサイト
* [Docker+Nginx+MySQLでLaravelの開発環境構築](https://entreprogrammer.jp/laravel-nginx-docker/)
* [Laravel公式のNginxのconfを解説・設定変更する](https://entreprogrammer.jp/laravel-nginx-conf/)


# 駄文
docker-compose.ymlで`env_file`で指定しても何故かうまく動いてくれないので下記のコマンドで使う`.env`ファイルを指定させた





