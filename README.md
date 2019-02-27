### ROLES:

| Role  | Operations |
| ------------- | ------------- |
| reader  | read  |
| writer  | read, write  |

### ACCOUNTS:

| Account  |
| ------------- |
| support  |
| cloud  |
| rnd  |


### USERS:

| User  | Accounts | Role | UserId |
| ------------- | ------------- | ------------- | ------------- |
| Иван | cloud, rnd, support | reader | 59afc932-a9c1-42f3-b024-525079ccd104 |
| Петр | cloud | writer | 46c75272-ec8d-4918-a445-358468d0ef95 |
| Петр | rnd | reader | 46c75272-ec8d-4918-a445-358468d0ef95 |
| Nikolas | cloud | reader | afd87e24-8b22-4635-889d-fc3125ac8f74 |

### RESOURCES

| Id  | type | caption | account |
| ------------- | ------------- | ------------- | ------------- |
| 2c568515-6a86-a7fb-3efd-cff97f7a759d | folder | RnD | rnd |
| f917f616-c9a5-750a-f814-189bff4fd24f | folder | Support | support |
| 584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4 | folder | Cloud | cloud |
| a0d83fad-a8a6-789f-9030-019037b9eadc | process | Автоматический обзвон | support |
| 5186961d-aa93-d419-1160-9291c3f98aed | process | Обратная связь с клиентом | support |
| ef8e43b2-7d8e-1714-2a73-2bc793312488 | process | Автом. обработка заявки | cloud |
| 19d469b9-f120-e04b-e98c-d0dd9edcc654 | process | Уведомление о проблемах с кластером ssd | cloud |
| 1d83ae7a-5ccd-80d1-fd4a-d45b65d14a0d | process | Напоминание о ревью кода | rnd |
| 1b2bd688-ce6c-fcd9-5d13-49c2db0cdda7 | process | Сбор статистики по коммитам | rnd |
| 042d7d27-33ad-031d-eee7-6703f594bb44 | process | Анализ ошибок кода | rnd |

### Examples

| Name  | HTTP method | user name | userId | body | account? | url |
| ------------- | ------------- | ------------- | ------------- | ------------- | ------------- | ------------- |
| Дай все документы для чтения | GET | Nikolas | afd87e24-8b22-4635-889d-fc3125ac8f74 | - | - | http://46.101.67.95/all?userId=afd87e24-8b22-4635-889d-fc3125ac8f74 |
| Доступность документа, для записи | GET | Петр | 46c75272-ec8d-4918-a445-358468d0ef95 | {"data":{"caption":"my_process in rnd","account":"cloud","parentId":"65ba63de-8ec4-4a40-a317-c11c172cb413"}} | cloud | http://46.101.67.95/?userId=46c75272-ec8d-4918-a445-358468d0ef95&securityTag=cloud |
| Доступность документа, для записи | GET | Петр | 46c75272-ec8d-4918-a445-358468d0ef95 | - | - |  |
