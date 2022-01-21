composer create-project symfony/skeleton blog-api
cd blog-api
git init
git remote add origin git@github.com:loic-cotty/blog-api.git
git add .
git commit -m "first commit"

composer require profiler --dev

composer require api

composer require logger

