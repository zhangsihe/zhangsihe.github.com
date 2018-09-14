
    1.vendor目录已经存在
    
    如果已经执行了composer update/install，需要先删除vendor目录 执行：rm -rf vendor
    git add -A
    git commit -m "remove vendor"
    composer update --prefer-dist
    git add . -A 
    git commit -m "recover vendor"
    
    2.vendor目录不存在
    
    composer update --prefer-dist
    git add . -A 
    git commit -m "recover vendor"