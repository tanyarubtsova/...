+ Lab: SQL injection vulnerability allowing login bypass
  + Открываем форму для ввода логина и пароля.
  + В поле Login вводим "administrator'-- ", а в поле Password любые символы.
  + WIN.
+ Lab: SQL injection UNION attack, finding a column containing text
  + Переходим в один из разделов, например Gifts.
  + В строке urla дописываем "'+UNION+SELECT+NULL--". Ошибка => дописываем еще NULL.
  + В итоге для urla с дописанной строкой "'+UNION+SELECT+NULL,+NULL,+NULL--" ошибки нет.
  + Вместо каждого NULL подставляем 'a'.
  + Для "'+UNION+SELECT+NULL,+'a',+NULL--" ошибки нет, нашли столбец с текстовыми данными.
  + Вместо 'a' вводим предложенну строку ('sypRvz').
  + WIN.
