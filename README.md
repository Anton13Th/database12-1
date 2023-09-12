# Домашнее задание по лекции "Базы данных" - 'Нагорнов Антон Алексеевич'

### Задание 1

Сотрудники (  
- employers_id, первичный ключ, serial  
- Lastname, varchar(50)  
- Firstname, varchar(50)  
- Midname, varchar(50)  
- date_start, date  
- position_id, int, внешний ключ -- Должность (pos_id)  
- division_id, int, внешний ключ -- Подразделение (div_id)  
- project_id, int, внешний ключ -- Проект (proj_id)  

Должность (  
- pos_id, первичный ключ, serial  
- position_name, varchar(50)  
- salary, money  

Подразделение (  
- div_id, первичный ключ, serial  
- div_name, varchar(100)  
- div_type, int, внешний ключ -- Тип подразделения (deptype_id)  

Тип подразделения (  
- deptype_id, первичный ключ, serial  
- deptype_name, varchar(100)  

Адреса (  
- address_id, первичный ключ, serial  
- area_id, внешний ключ -- Регион (region_id)  
- city_id, внешний ключ -- Города (cities_id)  

Регион (  
- region_id, первичный ключ, serial  
- region_name, varchar(100)  

Города (  
- cities_id, первичный ключ, serial  
- cities_name, varchar(255)  

Проект (  
- proj_id, первичный ключ, serial  
- project_name, varchar(100)  
