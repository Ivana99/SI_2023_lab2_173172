Втора лабораториска вежба по Софтверско инженерство
______________________________________________________

Ивана Стојановска, бр. на индекс 173172
______________________________________________________

Control Flow Graph
![image](SILab2_final.drawio.png)

Цикломатска комплексност

- Цикломатска комплексност на овој код е 11 , ја добив така што ги избројав регионите од Control
Flow графикот.

Multiple Condition критериумот за условот
if (user==null || user.getPassword()==null || user.getEmail()==null).

- За дадениот услов имаме 4 тест случаеви каде што: 
   1. user = null
   2. user = new User(); user.setPassword(null)
   3. user = new User(); user.setPassword("password"); user.setEmail(null);
   4. user = new User(); user.setPassword("password"); user.setEmail("user@example.com"); 

Тест случаи според критериумот Every branch
1. Тест во кој ќе се фрли exception пр: сите или едно се null (user==null || user.getPassword()==null || user.getEmail()==null) 
2. Тест  во кој username и password се исти со веќе постоечки корисници пр: username = 'Ivana', password = 'Ivana' , под претпоставка дека Ivana e веќе username на некој корисник
3. Тест во кој password има празно место пр: password = 'Iva na'
4. Тест во кој password нема празно место и нема специјален знак пр: password = 'Ivana'
5. Тест во кој password го содржи Usernam-от и е помал од 8 карактери
6. Тест во кој email содржи @ и . 
