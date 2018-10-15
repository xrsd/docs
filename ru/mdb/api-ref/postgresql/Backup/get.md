# Метод get
Возвращает указанный ресурс Backup для PostgreSQL.
 
Чтобы получить список доступных ресурсов Backup для PostgreSQL,
отправьте запрос [list](/docs/mdb/api-ref/postgresql/Backup/list).
 
## HTTP-запрос
`GET /managed-postgresql/v1/backups/{backupId}`
 
## Path-параметры {#path_params}
 
Name | Description
--- | ---
backupId | Обязательное поле. Идентификатор резервной копии, сведения о котором запрашиваются. Чтобы получить идентификатор резервной копии, используйте запрос [listBackups](/docs/mdb/api-ref/postgresql/Cluster/listBackups).
 
## Ответ {#responses}
**HTTP Code: 200 - OK**

Ресурс Backup для PostgreSQL. Подробнее см. в разделе [Взаимосвязь ресурсов сервиса](/docs/mdb/concepts).
 
Поле | Описание
--- | ---
id | **string**<br><p>Идентификатор резервной копии.</p> 
folderId | **string**<br><p>Идентификатор каталога, которому принадлежит резервная копия.</p> 
createdAt | **string** (date-time)<br><p>Время создания в формате <a href="https://www.ietf.org/rfc/rfc3339.txt">RFC3339</a> (т. е. когда операция резервного копирования была завершена).</p> 
sourceClusterId | **string**<br><p>Идентификатор кластера PostgreSQL, для которого была создана резервная копия.</p> 
startedAt | **string** (date-time)<br><p>Время запуска операции резервного копирования.</p> 