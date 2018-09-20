# Welcome to CodeBattle: Лунолет

## Как это подключить бота?
Необходимо подключиться из кода бота к серверу через вебсокет по адресу:
`ws://${server_host}:${server_port}/codebattle/ws?user=${email}&code=${auth_code}`
- `email` - email, указанынй при регистрации
- `code` - автоматически сгенерированный код. Виден в query parameters в адресной строке браузера *(после регистрации)*

В нашем случае мы используем сервер `http://server.codebattle.ru/codebattle`
- ${server_host} = server.codebattle.ru
- ${server_port} = 80

После подключения, клиент через вебсокет будет регулярно (каждую секунду) получать строку символов с закодированным состоянием игрового поля. 
Более подробно с правилами игры можно ознакомиться на [странице](Rules.md)

## 

#### Примеры клиентов (ботов)
- Java - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleJava 
- JavaScript - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleJS
- C# - https://github.com/IzhevskCodeBattle/codebattle-lunolet-clients/tree/master/CodeBattleNet

### [Правила игры](Rules.md)

### Сервер
- http://server.codebattle.ru/codebattle

