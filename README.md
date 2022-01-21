composer create-project symfony/skeleton blog-api
cd blog-api
git init
git remote add origin git@github.com:loic-cotty/blog-api.git
git add .
git commit -m "first commit"

composer require profiler --dev
composer require api
composer require logger
symfony composer req maker --dev
symfony composer req annotations

init bdd:
.env : mysql://root:MysqlPass!@127.0.0.1:3306/blog?serverVersion=5.7
bin/console doctrine:database:create

symfony console make:entity category
symfony console make:migration


