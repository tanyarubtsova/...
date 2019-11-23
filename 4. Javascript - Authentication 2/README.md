1) Переходим по адресу http://challenge01.root-me.org/web-client/ch11/
2) Видим кнопку login
3) Нажимаем клавиши Ctrl+Shift+i, внизу страницы открываем файл login.js
4)
```
var username = prompt("Username :", ""); //по сути строка username пустая
var password = prompt("Password :", "");
var TheLists = ["GOD:HIDDEN"]; // это список из 1 элемента-строки
for (i = 0; i < TheLists.length; i++) { //из предыдущей строки следует, что цикл выполняется только 1 раз
if (TheLists[i].indexOf(username) == 0) { //поиск в строке ["GOD:HIDDEN" пустой подстроки, вернувшийся индекс равен 0 => заходим в ветку if (не else)
var TheSplit = TheLists[i].split(":"); //разделили строку на две, записали из в массив
var TheUsername = TheSplit[0]; // ="GOD"
var ThePassword = TheSplit[1]; // ="HIDDEN"
if (username == TheUsername && password == ThePassword)
```
Вводим соответствующие значения логина (GOD), затем пароля (HIDDEN)
5) WIN 
