# OTUS_Postman
Ссылка на Сhallenges https://apichallenges.herokuapp.com/gui/challenges/2db27b14-daa4-4357-a1d2-031741f536ca

Задание со звездочкой: Для сайта https://try.vikunja.io подготовьте три рабочих GET запроса и два рабочих PUT запроса.

*1.  ПРОСМОТРЕТЬ СПИСОК ЗАДАЧ

   "see_List - GET lists/6"

curl --location --request GET 'https://try.vikunja.io/api/v1/lists/6' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":6,"title":"List1","description":"","identifier":"","hex_color":"","namespace_id":5,"owner":{"id":3,"name":"","username":"test1339","created":"2022-07-02T12:44:06+02:00","updated":"2022-07-02T12:44:06+02:00"},"is_archived":false,"background_information":null,"background_blur_hash":"","is_favorite":false,"position":393216,"created":"2022-07-02T12:50:04+02:00","updated":"2022-07-02T14:02:24+02:00"}
'

*2. ПРОСМОТРЕТЬ ЗАДАЧУ

"see_Task - GET tasks/26"

curl --location --request GET 'https://try.vikunja.io/api/v1/tasks/26' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":26,"title":"task2","description":"","done":false,"done_at":"0001-01-01T00:00:00Z","due_date":"0001-01-01T00:00:00Z","reminder_dates":null,"list_id":6,"repeat_after":0,"repeat_mode":0,"priority":0,"start_date":"0001-01-01T00:00:00Z","end_date":"0001-01-01T00:00:00Z","assignees":null,"labels":null,"hex_color":"","percent_done":0,"identifier":"-2","index":2,"related_tasks":{},"attachments":null,"is_favorite":false,"created":"2022-07-02T14:02:15+02:00","updated":"2022-07-02T14:02:15+02:00","bucket_id":10,"position":32768,"kanban_position":1703936,"created_by":{"id":3,"name":"","username":"test1339","created":"2022-07-02T12:44:06+02:00","updated":"2022-07-02T12:44:06+02:00"}}
'


*3. ПРОСМОТРЕТЬ КОМАНДУ

"see_Team- GET teams/3"

curl --location --request GET 'https://try.vikunja.io/api/v1/teams/3' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDkzODUyLCJpZCI6MiwiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOTAifQ.NG3u_FtLBwK-3XEyMd5zVDoAvsksefUSQXZ_MTzITME' \
--header 'Content-Type: application/json' \
--data-raw '{"id":3,"name":"Team1","description":"","created_by":{"id":2,"name":"","username":"test13390","created":"2022-07-03T09:50:47+02:00","updated":"2022-07-03T09:50:47+02:00"},"members":[{"id":2,"name":"","username":"test13390","created":"2022-07-03T09:50:47+02:00","updated":"2022-07-03T09:50:47+02:00","admin":true}],"created":"2022-07-03T09:52:51+02:00","updated":"2022-07-03T09:52:51+02:00"}'


*4. СОЗДАТЬ ЗАДАЧУ

"create_Task - PUT lists/10"

curl --location --request PUT 'https://try.vikunja.io/api/v1/lists/10' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":40,"title":"Task 2.3","description":"","done":false,"done_at":"0001-01-01T00:00:00Z","due_date":"0001-01-01T00:00:00Z","reminder_dates":null,"list_id":10,"repeat_after":0,"repeat_mode":0,"priority":0,"start_date":"0001-01-01T00:00:00Z","end_date":"0001-01-01T00:00:00Z","assignees":[],"labels":[],"hex_color":"","percent_done":0,"identifier":"-1","index":1,"related_tasks":{},"attachments":[],"is_favorite":false,"created":"2022-07-02T18:28:06.700994159+02:00","updated":"2022-07-02T18:28:06.701000978+02:00","bucket_id":14,"position":65536,"kanban_position":65536,"created_by":{"id":3,"name":"","username":"test1339","created":"2022-07-02T12:44:06+02:00","updated":"2022-07-02T12:44:06+02:00"}}
'


*5. ДОБАВИТЬ КОММЕНТАРИЙ К ЗАДАЧЕ

"add_comment - PUT tasks/17/comments"

curl --location --request PUT 'https://try.vikunja.io/api/v1/tasks/17/comments' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDkzODUyLCJpZCI6MiwiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOTAifQ.NG3u_FtLBwK-3XEyMd5zVDoAvsksefUSQXZ_MTzITME' \
--header 'Content-Type: application/json' \
--data-raw '{"id":2,"comment":"Comment 1234","author":{"id":2,"name":"","username":"test13390","created":"2022-07-03T09:50:47+02:00","updated":"2022-07-03T09:50:47+02:00"},"created":"2022-07-03T10:25:51.029610002+02:00","updated":"2022-07-03T10:25:51.029620552+02:00"}'

**
6. ДОБАВИТЬ СПИСОК ЗАДАЧ В ИЗБРАННОЕ

"iist_is_favorite - POST lists/6"

curl --location --request POST 'https://try.vikunja.io/api/v1/lists/6' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":6,"title":"List1","description":"","identifier":"","hex_color":"","namespace_id":5,"owner":{"id":3,"name":"","username":"test1339","created":"2022-07-02T12:44:06+02:00","updated":"2022-07-02T12:44:06+02:00"},"is_archived":false,"background_information":null,"background_blur_hash":"","is_favorite":true,"position":393216,"created":"2022-07-02T12:50:04+02:00","updated":"2022-07-02T13:42:57+02:00"}
'


**7. ДОБАВИТЬ ОПИСАНИЕ К ЗАДАЧЕ

"create_description - POST tasks/25"

curl --location --request POST 'https://try.vikunja.io/api/v1/tasks/25' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":25,"title":"task1","description":"Description 1.12","done":false,"done_at":"0001-01-01T00:00:00Z","due_date":"0001-01-01T00:00:00Z","reminder_dates":null,"list_id":6,"repeat_after":0,"repeat_mode":0,"priority":0,"start_date":"0001-01-01T00:00:00Z","end_date":"0001-01-01T00:00:00Z","assignees":[],"labels":null,"hex_color":"","percent_done":0,"identifier":"","index":1,"related_tasks":{},"attachments":null,"is_favorite":false,"created":"2022-07-02T14:52:36+03:00","updated":"2022-07-02T13:54:40+02:00","bucket_id":10,"position":65536,"kanban_position":65536,"created_by":{"id":3,"name":"","username":"test1339","created":"2022-07-02T10:44:06Z","updated":"2022-07-02T10:44:06Z"}}
'
