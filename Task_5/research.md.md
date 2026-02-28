### 1-Window Functions vs GROUP BY:

GROUP BY: 



لما تستخدم GROUP BY

إنت كده بتعمل aggregation per group

يعني كل جروب بيطلع صف واحد بس.



&nbsp;التفاصيل الأصلية بتختفي

&nbsp;النتيجة بتبقى على مستوى الجروب مش الصف



Window Functions: 

دي بتعمل aggregation برضه

بس من غير ما تمسح الصفوف الأصلية.



&nbsp;كل row بيفضل موجود

&nbsp;بس بيتضاف له عمود محسوب



### 2-Clustered vs Non-Clustered Indexes:

Clustered	                    |                                Non-Clustered

Leaf Nodes = Actual Data Rows         |            	Leaf Nodes = Key + Pointer

الداتا نفسها متخزنة في الشجره      	      بس مرجع لمكان الداتا                                               

الجدول نفسه مترتب على حسبه	الجدول مش مترتب عليه   





### 3-Filtered \& Unique Indexes:



Filtered Index



أصغر في الحجم



أسرع للـ queries اللي على شرط معين



بيقلل storage و I/O



Unique Index



يمنع التكرار



يبطّأ INSERT عشان بيعمل validation



يسرّع SELECT عشان البحث بيبقى direct ومضمون نتيجة واحدة





### 4-Choosing the Right Index:



Structure     	  لي               -             مناسب؟    - 

-------------------------------------------------------------------------------------------------

Heap	           ✅ أفضل اختيار	أسرع Insert وأقل Overhead

Clustered	 ❌   	بيحافظ على ترتيب فبيبطّأ                    

Non-Clustered	❌	                    Maintenance زيادة بدون فايدة

&nbsp;                           





### 5-Database Transactions (ACID):

&nbsp;             Atomicity بتحميك من:



فقدان بيانات



أرقام غلط



Inconsistent state



مشاكل مالية خطيرة



يعني ببساطة:



Either everything happens or nothing happens 

