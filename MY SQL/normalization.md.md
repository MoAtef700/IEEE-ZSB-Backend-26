##### 1NF :   

###### &nbsp;     الهدف من 1 NF:

###### 

###### \- إزاله القيم المتكررة أو المركّبة داخل نفس العمود

###### \- جعل كل صف وعمود يحتوي قيمة واحدة فقط

&nbsp;      



&nbsp; sol: We separate phone numbers into a new table. 







##### 2NF: 



##### 2NF بتعالج مشكلة اسمها Partial Dependency 





sol : We separate student data from course data.



##### 3NF : 



##### ما يكونش عندك اعتماد غير مباشر (Transitive Dependency) بين الأعمدة.





sol : We separate department information into its own table.









final result :




Students: 



Student\_ID (PK)



Student\_Name



City



Street



Zip







Student\_Phones:



Phone\_ID (PK)



Student\_ID (FK)



Phone\_Number







Courses:



Course\_ID (PK)



Course\_Title   











Instructors:



Instructor\_ID (PK)



Instructor\_Name



Dept\_ID (FK)







Departments:



Dept\_ID (PK)



Dept\_Name



Dept\_Building



Student\_Courses



Student\_ID (FK)



Course\_ID (FK)



Grade

