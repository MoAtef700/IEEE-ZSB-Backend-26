##### 1\. What is the difference between a DBMS and an RDBMS?

&nbsp;  answer/ DBMS : هو سيستم بيحفظ الداتا وخلاص، ومش شرط تكون الداتا مترابطة بجداول



&nbsp;                    RDBMS : بيخزن بيانات في جداول مرتبطه ببعض بقواعد منظمة. -

&nbsp;       زي: \*\*MySQL, SQL Server, Oracle, PostgreSQL\*\*

&nbsp;       



##### 2.difference

##### between DDL  and DML ? Give one example command for

##### each.

&nbsp;                    1-DML – Data Manipulation Language : تُستخدم للتعامل مع البيانات داخل الجداول

&nbsp;                                              

&nbsp;                                             INSERT  -  UPDATE - DELETE



&nbsp;						INSERT INTO Students (id, name)

&nbsp;						VALUES (1, 'Ali');



&nbsp;        2-  DDL – Data Definition Language :  تُستخدم لإنشاء أو تعديل أو حذف الجداول والهياكل في قاعدة البيانات 

&nbsp;                                          

&nbsp;                                          CREATE  -  ALTER   -   DROP   -  TRUNCATE

&nbsp;					      CREATE TABLE Students (

                                              id INT PRIMARY KEY,

    					      name VARCHAR(50)

 					      );





##### 3\. In your own words, why is Normalization important for a

##### large system like a university database?

&nbsp;  		Normalization بتخلي قاعده البيانات 

&nbsp;			1  منظمة  -

&nbsp;			2مفيهاش تكرار-

&nbsp;			3سهلة التعديل- 



