# Домашнее задание по лекции "Базы данных" - 'Нагорнов Антон Алексеевич'

### Задание 1

Сотрудники (  
- employers_id, первичный ключ, serial  
- fio, varchar(50)  
- date_start, date  
- position_id, int, внешний ключ -- Должность (pos_id)  
- division_id, int, внешний ключ -- Подразделение (div_id)  
- filial_id, int, внешний ключ -- Филиал (fil_id)  
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

Филиал (  
- fil_id, первичный ключ, serial  
- address_id, int, внешний ключ -- Адреса (address_id)  
- project_region_id, int, внешний ключ -- Регион (region_id)  

Адреса (  
- address_id, первичный ключ, serial  
- address_area, varchar(50)  
- address_city, varchar(50)  
- address_street, varchar(50)  
- address_building, varchar(10)  

Регион (  
- region_id, первичный ключ, serial  
- region_name, varchar(100)  

Проект (  
- proj_id, первичный ключ, serial  
- project_name, varchar(100)  
