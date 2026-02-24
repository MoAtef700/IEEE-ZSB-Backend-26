##### 1\. UNION vs UNION ALL:



Duplicate Handling – التعامل مع التكرارات



UNION



بيشيل أي صف مكرر automatically.



يعني النتايج اللي هترجع كلها unique.



بيعمل sort أو hash جوه عشان يشيل التكرارات.



UNION ALL



ما بيشيلش duplicates.



بيرجع كل الصفوف زي ما هي، حتى لو متكررة.



بس بيضم النتائج ببساطة





Performance – الأداء



UNION



أبطأ

عشان لازم يقارن كل الصفوف ويشيل التكرارات.

فيه overhead من sorting أو hashing.



UNION ALL



أسرع 

لأنه مش بيشيك علي duplicates

بس بيجمع النتائج على طول.





##### 2\. Subquery vs JOIN:





الأداء / Performance



JOIN: أسرع، ممكن يستخدم indexes كويس



Subquery: أبطأ خصوصًا لو correlated، لأنه بيتنفذ لكل صف



تحسين الأداء / Optimization



JOIN: DB engine optimized عليه كويس



Subquery: أقل قابلية للتحسين، ممكن الـ optimizer ما يستفيدش



التعامل مع الداتا الكبيرة / Scalability



JOIN: أفضل



Subquery: ممكن يكون بطيء مع large datasets



سهولة القراءة / Readability



JOIN: أوضح، العلاقات بين الجداول واضحة



Subquery: ممكن يكون معقد لو nested كتير



الاستخدام المناسب / Use case



JOIN: لما محتاج performance و scalable query



Subquery: لما محتاج EXISTS، NOT EXISTS، أو aggregate قبل join

