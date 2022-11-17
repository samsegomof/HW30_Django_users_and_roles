# HW_30_django_users_and_roles
## В данной работе:
- Пользователь наследуется от AbstractUser.
- Ролевая модель определена через собственное поле role с параметром choices.
- Доступы регулируются через Permissions.
- permission_classes используются как на уровне класса (атрибутом класса), так и на уровне метода (декоратором).
- CRUD методы CategoryView переписаны на CategoryViewSet

## Запуск проекта:
1. Клониоровать репозиторий `git clone https://github.com/SamVanGonof/HW30_Django_users_and_roles.git`
2. Удалить миграции из ads/migrations и users/migrations.
3. Подключить PostgreSQL базу данных `docker run --name postgres -e POSTGRES_PASSWORD=postgres -d postgres`
4. Применить миграции `./manage.py makemigrations` и затем `./manage.py migrate`
5. Заполнить БД данными из фикстур находящихся в папке data в следующей последовательности:
    1) ./manage.py loaddata data/locations.json
    2) ./manage.py loaddata data/users.json
    3) ./manage.py loaddata data/categories.json
    4) ./manage.py loaddata data/ads.json

Тестировать удобно в Postman.
