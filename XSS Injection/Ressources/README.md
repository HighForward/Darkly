# SQL INJECTION

_/index.php?page=member_

#### Our first injection is:
```
1 OR 1=1
```

#### when decrypt it with ````md5```` we found ````false````

#### So we encrypte ````true```` with ````md5```` that give:

```b326b5062b2f0e69046810717534cb09```

#### Reload the page and an we get that alert
![image info](img.PNG)



## Good behavior
```
Never let value that provide from client side have an impact on the web app
```