# Welcome to CodeBattle: Lunolet
## Как это работает?
Необходимо подключиться из кода бота к серверу через вебсокет по адресу:
`ws://${server_host}:${server_port}/codenjoy-contest/ws?user=${email}&code=${auth_code}`
- `email` - email, указанынй при регистрации
- `code` - автоматически сгенерированный код. Виден в query parameters в адресной строке браузера *(после регистрации)*

После подключения, клиент через вебсокет будет регулярно (каждую секунду) получать строку символов с закодированным состоянием игрового поля. 
Само игровое поле извлекается из ответа сервера регулярным выражением:
```
^board=(.*)$
```

Более подробно с правилами игры можно ознакомиться на [странице](Rules.md)

#### Примеры клиентов (ботов)
- Java - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleJava 
- JavaScript - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleJS
- C# - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleNet

### Правила игры
- http://server.codebattle.ru:8080/codebattle/resources/help/lunolet.html

### Сервер
- http://server.codebattle.ru:8080/codebattle

