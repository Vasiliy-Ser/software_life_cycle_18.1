# Домашнее задание к занятию 18.1 «Жизненный цикл ПО» - Падеев Василий

![answer1]()

## Подготовка к выполнению

1. Получить бесплатную версию Jira - https://www.atlassian.com/ru/software/jira/work-management/free (скопируйте ссылку в адресную строку). Вы можете воспользоваться любым(в том числе бесплатным vpn сервисом) если сайт у вас недоступен. Кроме того вы можете скачать [docker образ](https://hub.docker.com/r/atlassian/jira-software/#) и запустить на своем хосте self-managed версию jira.  
2. Настроить её для своей команды разработки.  
3. Создать доски Kanban и Scrum.  
4. [Дополнительные инструкции от разработчика Jira](https://support.atlassian.com/jira-cloud-administration/docs/import-and-export-issue-workflows/).  

## Основная часть

Необходимо создать собственные workflow для двух типов задач: bug и остальные типы задач. Задачи типа bug должны проходить жизненный цикл:

1. Open -> On reproduce.  
2. On reproduce -> Open, Done reproduce.  
3. Done reproduce -> On fix.  
4. On fix -> On reproduce, Done fix.  
5. Done fix -> On test.  
6. On test -> On fix, Done.  
7. Done -> Closed, Open.   

Остальные задачи должны проходить по упрощённому workflow:

1. Open -> On develop.  
2. On develop -> Open, Done develop.  
3. Done develop -> On test.  
4. On test -> On develop, Done.  
5. Done -> Closed, Open.  

**Что нужно сделать**

1. Создайте задачу с типом bug, попытайтесь провести его по всему workflow до Done.   
2. Создайте задачу с типом epic, к ней привяжите несколько задач с типом task, проведите их по всему workflow до Done.   
3. При проведении обеих задач по статусам используйте kanban.   
4. Верните задачи в статус Open.  

Там где задача должна находится в двух категориях использовал подзадачи.

![answer1](https://github.com/Vasiliy-Ser/software_life_cycle_18.1/blob/c789ee281dde7b599ef8ce830837302ca3cf74ac/file/1.png)  
![answer1](https://github.com/Vasiliy-Ser/software_life_cycle_18.1/blob/c789ee281dde7b599ef8ce830837302ca3cf74ac/file/4.png)

5. Перейдите в Scrum, запланируйте новый спринт, состоящий из задач эпика и одного бага, стартуйте спринт, проведите задачи до состояния Closed. Закройте спринт.  

![answer1](https://github.com/Vasiliy-Ser/software_life_cycle_18.1/blob/c789ee281dde7b599ef8ce830837302ca3cf74ac/file/3.png)

6. Если всё отработалось в рамках ожидания — выгрузите схемы workflow для импорта в XML. Файлы с workflow и скриншоты workflow приложите к решению задания.  

![answer1](https://github.com/Vasiliy-Ser/software_life_cycle_18.1/blob/c789ee281dde7b599ef8ce830837302ca3cf74ac/file/2.png)

[Файлы с workflow](https://github.com/Vasiliy-Ser/software_life_cycle_18.1/blob/c789ee281dde7b599ef8ce830837302ca3cf74ac/file/Software%20Simplified%20Workflow%20for%20Project%20BUG8.xml)

---

### Как оформить решение задания

Выполненное домашнее задание пришлите в виде ссылки на .md-файл в вашем репозитории.

---
