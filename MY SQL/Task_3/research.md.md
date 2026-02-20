##### 1\. WHERE vs HAVING: Both are used to filter data, but they

##### are used in different places in a query. Explain the

##### difference between them and when to use which. (Give a

##### code example).  

&nbsp;   

###### &nbsp;               	ans/ WHERE: يفلتر الصفوف قبل التجميع.

###### &nbsp;                                         HAVING: يفلتر المجموعات بعد التجميع.







##### 

##### 2\. DELETE vs TRUNCATE vs DROP: We learned about deleting

##### data. What is the difference between these three

##### commands? Which one can be rolled back (undone)?    



&nbsp;	ans/      DELETE --> بيحذف صفوف -ممكن تحط شرط WHERE - يقدر يتعمله Rollback 



&nbsp;		 TRUNCATE --> بيمسح كل البيانات بسرعة - مفيش WHERE -  غالبًا لا يمكن Rollback - بيصفر الـ Auto Increment



&nbsp;		 DROP  --> بيمسح الجدول نفسه - البيانات + structure





##### 

##### 3\. Order of Execution: When you write a query like SELECT

##### ... FROM ... WHERE ... GROUP BY ... HAVING ... ORDER BY,

##### the database does not read it in that order. What is the

##### actual "Logical Order of Execution" that the SQL engine

##### performs?

1\. FROM

2\. WHERE

3\. GROUP BY

4\. HAVING

5\. SELECT

6\. ORDER BY

7\. LIMIT



##### 

##### 4\. COUNT(\*) vs COUNT(Column\_Name): In aggregation, these

##### two look similar but behave differently regarding NULL

##### values. What is the exact difference?



COUNT(\*)

بيعد كل الصفوف حتى لو فيها NULL



OUNT(column\_name)

بيعد القيم اللي مش NULL 





##### 5\. CHAR vs VARCHAR: Both store text, but they manage

##### storage space differently. Explain the difference

##### between CHAR(10) and VARCHAR(10) if we store the word

##### "Cat" in both.

&nbsp; ans / CHAR(10) :حتي لو الكلمه اقل من عشره  دايمًا يحجز 10 حروف 

&nbsp;          	VARCHAR(10)    يحجز على قد الكلمة بس حتي لو اقل من عشره  : 







