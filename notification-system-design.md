# Notification System Design
Campus Notifications Microservice

Stage 3

 ----> Yes,the query is accurate but it is slow because retreiving information using studentId and boolean variable isRead takes time as there are 5000000 students data.
 ----->The change I would recommend is to use indexes to make searching faster
 ------> The suggestion given by another developer in creating indexes is a efficient advice 

 QUERY
  SELECT * FROM  notifications WHERE notification_type(SELECT * FROM notifications ORDER BY Placements DESC LIMIT 7);
