## Calendário

`[prompt]# cal` → mostra o calendário

`[prompt]# cal 01 2020` → especifica mês e ano a ser mostrado

→ `<comando> | more` a lista a seguir vira em telas quebradas (páginas).


## Data

`[prompt]# date`

`[prompt]# date 032510232019 | hwcloack -w` → atualiza data e hora sendo:

`03` → mês

`25` → dia

`10` → hora 

`23` → minutos

`2019` → ano

`hwcloack -w` → (hardware cloak) responsável por registrar!



`[prompt]# date + %d / %m / %y` → 01 / 08 / 19
`[prompt]# date + %d / %m / %Y` → 01 / 08 / 2019
`[prompt]# date + %H : %M : %S` → 14 : 20 : 52 
`[prompt]# date "+ %d / %B / %Y"` → 01 agosto 2019
`[prompt]# date "+ %d / %B / %Y, %A"` → 01 agosto 2019, quinta


## Impressora