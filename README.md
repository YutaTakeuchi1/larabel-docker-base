DockerでLarabel + mariaDB + Apache環境を構築する練習をしたもののバックアップです。

#パーミッションエラーが出た場合以下のコマンドを実行  
``docker-compose run php chmod -R 0777 /var/www/html/bootstrap``  
``docker-compose run php chmod -R 0777 /var/www/html/storage``

#忘備録  
``docker-compose run php composer create-project --prefer-dist laravel/laravel .``

``docker exec -it laravel-php bash``  
``php artisan migrate``  
``php artisan migrate:rollback``
