# Password_Recovering

_/index.php?page=recover_

#### A formdata is sent with an email that will be used to recover a password, we can change the mail value with an API request
```curl --location 'http://192.168.1.27/index.php?page=recover' --form 'mail="another_email"' --form 'Submit="Submit"'```

#### We get the flag
```
<h2 style="margin-top:50px;"> The flag is : 1d4855f7337c0c14b6f44946872c4eb33853f40b2d54393fbe94f49f1e19bbb0</h2>
```

## Good behavior
```
Never allow user from client side to access/modify sensitive data
```