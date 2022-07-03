# OTUS_Postman
1.  ПОСМОТРЕТЬ СПИСОК ЗАДАЧ ПОД НАЗВАНИЕМ List1
   see_List - GET lists/6

curl --location --request GET 'https://try.vikunja.io/api/v1/lists/6' \
--header 'Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6InRlc3QxMzM5QGdtYWlsLnJ1IiwiZW1haWxSZW1pbmRlcnNFbmFibGVkIjpmYWxzZSwiZXhwIjoxNjU3MDIwMTM3LCJpZCI6MywiaXNMb2NhbFVzZXIiOnRydWUsImxvbmciOmZhbHNlLCJuYW1lIjoiIiwidHlwZSI6MSwidXNlcm5hbWUiOiJ0ZXN0MTMzOSJ9.3jF8-PYVBRdZdWo4QTOWqOmWWQTwf8E67DN6LA6Cv9k' \
--header 'Content-Type: application/json' \
--data-raw '{"id":6,"title":"List1","description":"","identifier":"","hex_color":"","namespace_id":5,"owner":{"id":3,"name":"","username":"test1339","created":"2022-07-02T12:44:06+02:00","updated":"2022-07-02T12:44:06+02:00"},"is_archived":false,"background_information":null,"background_blur_hash":"","is_favorite":false,"position":393216,"created":"2022-07-02T12:50:04+02:00","updated":"2022-07-02T14:02:24+02:00"}


'
