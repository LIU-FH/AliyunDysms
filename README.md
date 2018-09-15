# aliyunDysms
阿里云短信服务发送短信



require_once 'aliyunDysms/Dysms.php';

$Dysms = new \Dysms("yourAccessKeyId",'yourAccessKeySecret');

$data = array("code"=>"123456")// 短信模板中字段的值

return $Dysms->sendSms("短信接收号码",$data,"短信签名","模板CODE");
