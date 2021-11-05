淘宝开放平台SDK

## 安装

```
composer require yzh52521/open-taobao-sdk
```

### 使用

```php
<?php


$taobao = new \yzh52521\Taobao\Taobao(['key' => 'your-key', 'secret' => 'your-secret']);

// 使用如下
$taobao->request('method', $params);

// 例子
print_r($taobao->request('taobao.tbk.item.get', ['fields' => 'num_iid,title,pict_url,small_images,reserve_price,zk_final_price,user_type,provcity,item_url,seller_id,volume,nick', 'q' => '便利贴']));

```
