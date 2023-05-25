Втора лабораториска вежба по Софтверско инженерство
______________________________________________________

Ивана Стојановска, бр. на индекс 173172
______________________________________________________

Control Flow Graph

![Control Flow Graph](SI_2023_lab2_173172/SILab2.drawio.png)
SILab2.drawio.png

Цикломатска комплексност

- Цикломатска комплексност на овој код е 10 , ја добив така што ги избројав регионите од Control
Flow графикот + 1.

Multiple Condition критериумот за условот
if (user==null || user.getPassword()==null || user.getEmail()==null).

- За дадениот услов имаме 4 тест случаеви каде што: 
   1. user = null
   2. user = new User(); user.setPassword(null)
   3. user = new User(); user.setPassword("password"); user.setEmail(null);
   4. user = new User(); user.setPassword("password"); user.setEmail("user@example.com"); 

Тест случаи според критериумот Every statement
....

Тест случаи според критериумот Every path
....

Објаснување на напишаните unit tests
... ...
