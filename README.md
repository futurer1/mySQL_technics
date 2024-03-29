
![SQL Join operations](SQLjoins.png)


INNER JOIN
* пересечение – это результат операции inner join

![](innerJoin.jpg)

OUTER LEFT JOIN
* проводится проверка на соответствие условия соединения;
* если оно выполняется – строчка из второй прибавляется к первой таблице
* когда значение отсутствует в правой таблице, поля отображаются в виде null;
* если выставленный параметр слияния не выполняется, строчки отбрасываются.

![](outerLeftJoin.jpg)


OUTER RIGHT JOIN
* возвращаются все строки из правой таблицы
* дополнительно выводятся строчки левой таблицы, которые имеют с правой одинаковые значения;
* если поле из правой отсутствует в левой, соответствующие поля имеют значение null.

![](outerRightJoin.jpg)

FULL JOIN
* возвращаются все строчки из левой и правой таблиц со значениями null, когда условие не выполнено
* слияние двух множеств

![](outerFullJoin.jpg)

LEFT JOIN WITH NULL
* данные из первой таблицы, но исключая поля, совпадающие со второй таблицей
SELECT * FROM table1 LEFT JOIN table2 ON table1.id = table2.id WHERE table2.id IS NULL;

![](outerLeftJoinNull.jpg)
