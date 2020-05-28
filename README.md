[参考リンク](https://qiita.com/TAMIYAN/items/ed9ec892d91e5af962c6)
* dockerの環境構築方法
  1. docker-compose build
  2. docker-compose up -d
  3. docker exec -it docker-mysql_mysql_1 bash -p
  4. mysql -u root -p -h 127.0.0.1
  5. docker cp world.sql.zip docker-mysql_mysql_1:/
   
* dockerコンテナに入ってからやること
  1. apt update
  2. apt-get install unzip
  3. unzip world.sql.zip
  4. mysql -uroot -p  < world.sql