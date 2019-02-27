### ROLES:

| Role  | Operations |
| ------------- | ------------- |
| reader  | read  |
| writer  | read, write  |

### USERS:

| User  | Accounts | Role | UserId |
| ------------- | ------------- | ------------- | ------------- |
| Иван | cloud, rnd, support | reader | 59afc932-a9c1-42f3-b024-525079ccd104 |
| Петр | cloud | writer | 46c75272-ec8d-4918-a445-358468d0ef95 |
| Петр | rnd | reader | 46c75272-ec8d-4918-a445-358468d0ef95 |
| Nikolas | cloud | reader | afd87e24-8b22-4635-889d-fc3125ac8f74 |

### ACCOUNTS:

* support
* cloud
* rnd


RESOURCES FROM catalog service:
```
{
    "_id" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
    "type" : "folder",
    "caption" : "RnD",
    "account" : "rnd",
    "id" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "f917f616-c9a5-750a-f814-189bff4fd24f",
    "type" : "folder",
    "caption" : "Support",
    "account" : "support",
    "id" : "f917f616-c9a5-750a-f814-189bff4fd24f",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
    "type" : "folder",
    "caption" : "Cloud",
    "account" : "cloud",
    "id" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "a0d83fad-a8a6-789f-9030-019037b9eadc",
    "type" : "process",
    "caption" : "Автоматический обзвон",
    "account" : "support",
    "parentId" : "f917f616-c9a5-750a-f814-189bff4fd24f",
    "id" : "a0d83fad-a8a6-789f-9030-019037b9eadc",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "5186961d-aa93-d419-1160-9291c3f98aed",
    "type" : "process",
    "caption" : "Обратная связь с клиентом",
    "account" : "support",
    "parentId" : "f917f616-c9a5-750a-f814-189bff4fd24f",
    "id" : "5186961d-aa93-d419-1160-9291c3f98aed",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "ef8e43b2-7d8e-1714-2a73-2bc793312488",
    "type" : "process",
    "caption" : "Автом. обработка заявки",
    "account" : "cloud",
    "parentId" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
    "id" : "ef8e43b2-7d8e-1714-2a73-2bc793312488",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "19d469b9-f120-e04b-e98c-d0dd9edcc654",
    "type" : "process",
    "account" : "cloud",
    "caption" : "Уведомление о проблемах с кластером ssd",
    "parentId" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
    "id" : "19d469b9-f120-e04b-e98c-d0dd9edcc654",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "1d83ae7a-5ccd-80d1-fd4a-d45b65d14a0d",
    "type" : "process",
    "account" : "rnd",
    "caption" : "Напоминание о ревью кода",
    "parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
    "id" : "1d83ae7a-5ccd-80d1-fd4a-d45b65d14a0d",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "1b2bd688-ce6c-fcd9-5d13-49c2db0cdda7",
    "type" : "process",
    "account" : "rnd",
    "caption" : "Сбор статистики по коммитам",
    "parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
    "id" : "1b2bd688-ce6c-fcd9-5d13-49c2db0cdda7",
    "_type" : "http://sharejs.org/types/JSONv0"
}
{
    "_id" : "042d7d27-33ad-031d-eee7-6703f594bb44",
    "type" : "process",
    "account" : "rnd",
    "caption" : "Анализ ошибок кода",
    "parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
    "id" : "042d7d27-33ad-031d-eee7-6703f594bb44",
    "_type" : "http://sharejs.org/types/JSONv0"
}

```
