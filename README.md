# API Docs  
-------------  
## 1) Login  
```URL: https://sreeharis.tk/cc/login.php```  
```Method: POST```  
`username: your username`  
`password: SHA512 hash of password (all lowercase)`  
#### Return Values (JSON):  
`login: "fail"`  
`login:"pass", token:"some uuid"`  
save the uuid somewhere, as this is esentially a session ID  
## 2) Logout  
```URL: https://sreeharis.tk/cc/logout.php```  
```Method: POST```  
`uuid: Session ID from login`  
#### Return Values (JSON):  
None really that matter  
## 3) Get Messages
```URL: https://sreeharis.tk/cc/get.php```  
```Method: POST```  
`uuid: Session ID from login`  
`group: group name`  
#### Return Values (JSON):
`request`: `pass` or `fail`
`#`: one **message** (Replace `#` with a number
