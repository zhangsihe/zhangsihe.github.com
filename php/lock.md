    阻塞
    <?php
        $fp = fopen("lock.txt", "r");
        if(flock($fp,LOCK_EX))
        {
            // 处理相关逻辑
            flock($fp,LOCK_UN);
        }
        fclose($fp);
    ?>
    
    非阻塞
    <?php
        $fp = fopen("lock.txt", "r");
        if(flock($fp,LOCK_EX))
        {
            // 处理相关逻辑
            flock($fp,LOCK_UN);
        }
        fclose($fp);
     ?>