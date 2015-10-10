# hashidsDemo
hashidsDemo  里面有DEMO

$key = 'test';
$min_hash_length = 12;
$hashids = new Hashids($key,$min_hash_length);
//$ids = array(1,2,3);
$ids = array(134);
 // 加密
$str = $hashids->encode($ids);
echo $str."<br>";//exit;
 // 解密
$ids = $hashids->decode($str);
echo "<pre>";
var_dump($ids);
