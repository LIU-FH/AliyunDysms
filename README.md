# aliyunDysms
阿里云短信服务发送短信

require_once 'aliyunDysms/Dysms.php';

$Dysms = new \Dysms("yourAccessKeyId",'yourAccessKeySecret');

$TemplateCode = array('SMS_119075149');

return $Dysms->sendSms("短信接收号码",array(  // 短信模板中字段的值

            "code"=>"12345",
            
            "product"=>"dsd"
            
        ),"短信签名","模板CODE");
