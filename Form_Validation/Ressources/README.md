# Form_Validation

_/index.php?page=survey_

#### Un formdata est envoyé avec une value entre 1 et 10
```
If we send an API requests directly with CURL or Postman and modify the value
by something greater than 10, we get the flag
```

````curl --location 'http://192.168.1.27/index.php?page=survey' --form 'sujet="4"' --form 'valeur="11"'````

#### We get the flag
```
<h2 style="margin-top:50px;"> The flag is 03a944b434d5baff05f46c4bede5792551a2595574bcafc9a6e25f67c382ccaa</h2>
```

## Good behavior
```
Always validate values from client side before saving it in database or using it in any way
```