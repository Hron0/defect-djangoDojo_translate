# Для страта вам потребуется Docker desktop.

# Клонируем проект.
git clone https://github.com/GUDVIN18/defect-djangoDojo_v2

# Переходим в папку с проектом.
cd defect-djangoDojo_v2

# Сброка.
./dc-build.sh
# Запускаем все необходимые сервисы.
./dc-up-d.sh postgres-redis

# Получаем пароль для пользователя admin.
docker compose logs initializer | grep "Admin password:"

# Переходим по адресу 
http://localhost:8080/
