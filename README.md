# php-file-cache
### php 文件缓存类

#### 使用方式

```php
$cache = new FileCache();

$key = 'key';
$value = 'value';
// 缓存时间
$exprie = 3600;
$set = $cache->set($key, $value , $exprie);


// 获取缓存
$have = $cache->isHave($key);
if ($have){
    $get = $cache->get($key);

}else{

    echo '获取缓存失败';
    exit();
}

// 删除缓存
$delete = $cache->delete($key);

// 清空缓存
$flush = $cache->flush();
```
