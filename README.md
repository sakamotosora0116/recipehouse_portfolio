以下の技術を使用しております。

フロントエンド: tailwind,vue3,typescript 
バックエンド: laravel9
データベース: MySQL
Webサーバソフト：apache2
インフラ: AWS EC2

SPAのアプリとなっており、テーブル構造は
Category-Recipeの多対多となっております。（レシピからカテゴリへの参照は未実装です。）

テキストに値を入力すると画面右側にカテゴリが追加され、画面右側にあるテキストボックスから値を入力することでカテゴリに紐づいたレシピが追加されます。

カテゴリのタイトルをクリックすることで右画面がそのカテゴリに切り替わります。

右画面に表示されているカテゴリと同じカテゴリを削除すると、左画面からそのカテゴリが削除され、ひとつ上のカテゴリに移動します。それに伴い右画面もそのカテゴリを表示します。
このとき、削除したカテゴリにひもづいたレシピは削除されます。

すべてのカテゴリを削除すると、右画面にNot categoryと表示されます。

### 自分用

git clone したあとにやること一覧

php artisan key:generate

chmod -R 777 storage bootstrap/cache

sudo /opt/lampp/lampp start

mv .env.example .env

mysql 接続


npm run dev
php artisan serve
php artisan migrate

### todo 

soft deleting

pagination
