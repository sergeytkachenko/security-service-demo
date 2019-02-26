```
ROLES:
reader - read
writer  - read, write


USERS:
Иван - cloud, rnd, support - reader  - 59afc932-a9c1-42f3-b024-525079ccd104

Петр - cloud - writer  - 46c75272-ec8d-4918-a445-358468d0ef95
Петр - rnd - reader  -  46c75272-ec8d-4918-a445-358468d0ef95

Nikolas - cloud - reader  - afd87e24-8b22-4635-889d-fc3125ac8f74


ACCOUNTS:
  support
  cloud
  rnd


RESOURCES:
{
	"caption" : "R&D",
	"id" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
	"type" : "folder",
  "SecurityTags" : [
      "rnd"
  ]
},
{
	"caption" : "Support",
	"id" : "f917f616-c9a5-750a-f814-189bff4fd24f",
	"type" : "folder",
  "SecurityTags" : [
      "support"
  ]
},
{
	"caption" : "Cloud",
	"id" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
	"type" : "folder",
  "SecurityTags" : [
      "cloud"
  ]
},
{
	"caption" : "Автоматический обзвон",
	"id" : "a0d83fad-a8a6-789f-9030-019037b9eadc",
	"parentId" : "f917f616-c9a5-750a-f814-189bff4fd24f",
	"type" : "process",
  "SecurityTags" : [
      "support"
  ]
},
{
	"caption" : "Обратная связь с клиентом",
	"id" : "5186961d-aa93-d419-1160-9291c3f98aed",
	"parentId" : "f917f616-c9a5-750a-f814-189bff4fd24f",
	"type" : "process",
  "SecurityTags" : [
      "support"
  ]
},
{
	"caption" : "Автом. обработка заявки",
	"id" : "ef8e43b2-7d8e-1714-2a73-2bc793312488",
	"parentId" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
	"type" : "process",
  "SecurityTags" : [
      "cloud"
  ]
},
{
	"caption" : "Уведомление о проблемах с кластером ssd",
	"id" : "19d469b9-f120-e04b-e98c-d0dd9edcc654",
	"parentId" : "584b8b60-ca4b-8ee6-f7f9-3b55e8ab58b4",
	"type" : "process",
  "SecurityTags" : [
      "cloud"
  ]
},
{
	"caption" : "Напоминание о ревью кода",
	"id" : "1d83ae7a-5ccd-80d1-fd4a-d45b65d14a0d",
	"parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
	"type" : "process",
  "SecurityTags" : [
      "rnd"
  ]
},
{
	"caption" : "Сбор статистики по коммитам",
	"id" : "1b2bd688-ce6c-fcd9-5d13-49c2db0cdda7",
	"parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
	"type" : "process",
  "SecurityTags" : [
      "rnd"
  ]
},
{
	"caption" : "Анализ ошибок кода",
	"id" : "042d7d27-33ad-031d-eee7-6703f594bb44",
	"parentId" : "2c568515-6a86-a7fb-3efd-cff97f7a759d",
	"type" : "process",
  "SecurityTags" : [
      "rnd"
  ]
},
```
