# HW_30_django_users_and_roles
## В данной работе:
- Пользователь наследуется от AbstractUser.
- Ролевая модель определена через собственное поле role с параметром choices.
- Доступы регулируются через Permissions.
- permission_classes используются как на уровне класса (атрибутом класса), так и на уровне метода (декоратором).
- CRUD методы CategoryView переписаны на CategoryViewSet

## Запуск проекта:
1. Клониоровать репозиторий `git clone https://github.com/SamVanGonof/HW30_Django_users_and_roles.git`
