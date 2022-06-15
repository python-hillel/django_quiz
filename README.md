# Django QUIZ

## Технические требования  
### Web-UI
  1. Регистрация
      - регистрация (с подтверждением по email)
      - авторизация
      - смена пароля
      - сброс пароля
    
  2. Возможности пользоваля
      - прохождение любого теста
      - последовательно проходить вопросы теста (один за другим)
      - завершение отложенного теста
      - удаление незавершенного теста 
      - просмотр результатов
    
  3. После завершения теста
      - отчет о ко-ве правильных и неправильных ответов
      - процент правильных ответов

### Admin site
  1. Управление пользователями
  2. Управление тестами
      - добавление теста
      - изменить тест
      - удаление теста
      - валидация теста
        - нельзя сохранить вопрос:
            - без указания правильного ответа
            - в которов все ответы правильные

### Дополнительные требования
1. [x] Проект должен быть на Git-е
2. [x] Наличие файла requirements.txt
3. [x] venv
4. [ ] PostgreSQL
5. [ ] Наличие дампа данных
6. [ ] bootstrap
7. [ ] API + Tests
8. [ ] Docker image
9. [ ] Кэширование 
10. [ ] Планировщик
11. [ ] Деплой на Amazon

## DB - Schema
![db](db_schema.jpg)


## Lesson 01
- Создаём GIT репозиторий, клонируем его
- В клонированном репо создаём проект
- Устанавливаем Django и все необходимые зависимости
- Создаём приложения:
  - accounts
  - quiz
- Настраиваем проект
- Переопределяем модель User
- Создаём формы регистрации и редактирования пользователя
- Создаём view регистрации, активации и успешной активации
- Для отправки письма с приглашением активировать аккаунт, используем созданный сигнал
- Сообщаем Django о новой модели пользователя