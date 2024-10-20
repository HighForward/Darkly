# Form_Validation

/?page=b7e44c7a40c5f80139f0a50f3650fb2bd8d00b0d24667c4c2ca32c88e13b758f

#### There is a large comment on this page with somes informations:
```
<!--
    You must come from : "https://www.nsa.gov/".
    Let's use this browser : "ft_bornToSec". It will help you a lot.
-->
```

#### So we make thre requests with

````curl --location 'http://192.168.1.27/?page=b7e44c7a40c5f80139f0a50f3650fb2bd8d00b0d24667c4c2ca32c88e13b758f' --header 'Referer: https://www.nsa.gov/' --header 'User-Agent: ft_bornToSec'````

#### We get the flag
```
<h2 style="margin-top:50px;"> The flag is : f2a29020ef3132e01dd61df97fd33ec8d7fcd1388cc9601e7db691d17d4d6188</h2>
```

## Good behavior
```
Never show sensitives informations in comments, or allow client side 
```