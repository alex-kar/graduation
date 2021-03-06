# ВЫПУСКНОЙ ПРОЕКТ СТАЖИРОВКИ TOPJAVA

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/1af51a297ea24ae4ad39d3ef80fd6183)](https://app.codacy.com/app/alex-kar/Graduation?utm_source=github.com&utm_medium=referral&utm_content=alex-kar/Graduation&utm_campaign=Badge_Grade_Settings)
[![Build Status](https://travis-ci.org/alex-kar/Graduation.svg?branch=master)](https://travis-ci.org/alex-kar/Graduation)

### Деплой в Heroku: [GRADUATION](http://choice-restaurant.herokuapp.com).

Приложение с регистрацией/авторизацией и интерфейсом на основе ролей (USER, MANAGER, ADMIN).

**Администратор** может создавать/редактировать/удалять пользователей, изменять им роли, и временно отключать их.

**Менеджеры** могут создавать/редактировать/удалять рестораны, которыми они управляют, а также вести список блюд для каждого ресторана.
При этом они могут из общего списка блюд ресторана выбирать те из них, которые будут в меню сегодня и будут видны всем пользователям, в отличие от общего списка блюд.

**Пользователи** могут управлять своим профилем, просматривать общий список ресторанов и их сегодняшнее меню, и голосовать за понравившийся ресторан.
При этом у каждого пользователя только один голос в день, он может менять свой выбор по ходу дня, но в 18.00 по московскому времени голосование завершается.

Анонимным пользователям доступна только стартовая страница с возможностью зарегистрироваться.
Кроме того, для тестирования приложения возможен вход с главной страницы под любой из трех выбранных ролей.

Управление возможно через UI (по AJAX) и по REST интерфейсу с базовой авторизацией.  
Весь REST интерфейс покрывается JUnit тестами, используя Spring MVC Test и Spring Security Test.  
Реализованы базовая интернационализация, кэширование основных запросов, валидация вводимых пользователем данных и обработка ошибок.

### Стек технологий

- Spring Framework, Spring Data JPA, Spring MVC, Spring Security, Spring Test
- Hibernate ORM, Hibernate Validator, HSQLDB, PostgreSQL
- JUnit, AssertJ, Hamcrest
- Jackson, EhCache, Logback, SLF4J
- Apache Tomcat, JSP, JSTL
- Jquery, Jquery Datatables, Bootstrap