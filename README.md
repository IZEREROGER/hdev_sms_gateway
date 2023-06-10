
# HDEV SMS GATEWAY

### HADEV SMS. MIT license.

Use from a PHP script:


# INitiate sms
```php
include 'sms_parse.php';

//SEND SMS

hdev_sms::api_id("Your Api ID");
hdev_sms::api_key("Your Api Key");
$msg = hdev_sms::send("SENDER ID","TELL","MESSAGE");

var_dump($pay);//to get sms server response
```

# TOP UP 
```php
include 'sms_parse.php';

//TOP UP

hdev_payment::api_id("Your Api ID");
hdev_payment::api_key("Your Api Key");
$result = hdev_payment::topup($tel,$amount);

var_dump($result);//to get sms server response
```

*All of our response are objects for example to access the status in response you use
```php
	$status = $result->status;
```
