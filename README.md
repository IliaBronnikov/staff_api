## API для представления структуры компании:
- Список сотрудников (как общий, так и по департаментам отдельно)
- Список департаментов

### Установка проекта

- Собрать образ 
```
docker-compose up
```
- Образ postgres работает на порту 5432
- Сервис доступен по адресу http://127.0.0.1:8000/

### Документация по API
- /swagger

#### Endpoints:
- /staff/ - получение списка всех сотрудников с возможностью фильтрации по фамилии и департаменту
- /staff/<int:pk>/ - удаление сотрудника из БД
- /department/ - получение списка всех департаментов, включая искусственное поле с числом сотрудников и суммарным окладам по всем сотрудникам


