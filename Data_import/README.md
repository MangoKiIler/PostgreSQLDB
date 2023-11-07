# Существует ещё вариант импорта данных из файлов формата .csv.
Этим вариантом можно воспользоваться в том случае, если уже имеются подготовленные файлы для импорта.

Чтобы импортировать данные из файлов в пустые таблицы бд, необходимо для каждого файла запускать скрипт, где указывается в какую таблицу должны импортировать данные, а потом полный путь, где находится этот файл с данными. 
Также указывается символ разделения столбцов и заголовок. 


COPY post(post_name) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\post_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY employees(employee_name, employee_surname, employee_midname, date_of_birth, phonenum, passport, id_name_post) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\employees_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY customer(customer_name, customer_surname, customer_midname, date_of_birth, phonenum, passport) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\customer_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY newspaper_number(release_date) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\newspaper_number_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY articles(id_employees, id_customer, id_newspaper_number, article_name, public_date, price) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\articles_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY tags(tags_name) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\tags_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------
COPY article_tag(id_articles, id_tags) FROM 'C:\Users\НАВАЗНИЕ ВАШЕГО АККАУНТА\Desktop\course_work\datas\article_tag_data.csv' DELIMITER ',' CSV HEADER;
--------------------------------------------------------------------------------------------------

