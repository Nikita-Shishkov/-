otvet na zadanie 1:

SELECT task_status.issue_key AS number, task_info.name AS name, task_info.type AS type, task_status.status AS status, task_status.start_time AS time FROM task_status INNER JOIN task_info ON task_info.issue_key = task_status.issue_key WHERE task_info.type = 'Bug' AND task_status.status = 'in progress' AND task_status.start_time >= '2021-04-01' AND task_status.start_time < '2021-05-01';

Dlya udobstva chteniya koda:

SELECT

task_status.issue_key AS number,

task_info.name AS name,

task_info.type AS type,

task_status.status AS status,

task_status.start_time AS time

FROM

task_status

INNER JOIN task_info ON task_info.issue_key = task_status.issue_key 

WHERE

task_info.type = 'Bug' AND task_status.status = 'in progress' AND task_status.start_time >= '2021-04-01' AND task_status.start_time < '2021-05-01';



otvet na zadanie 2:

Dlya proverki skidki 1 % mozhno vzyat` testovye dannye 55, 0, 1, 98, 99.

Dlya proverki skidki 3 % mozhno vzyat` testovye dannye 140, 100,101,198,199.

Dlya proverki skidki 5 % mozhno vzyat` testovye dannye 251, 200,201,498,499.

Dlya proverki skidki 10 % mozhno vzyat` testovye dannye 678, 500, 501.
