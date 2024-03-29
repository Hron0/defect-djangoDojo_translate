# Для страта вам потребуется Docker desktop

# Клонируем проект
git clone https://github.com/GUDVIN18/defect-djangoDojo_v2
cd django-DefectDojo_v2

# Сброка
./dc-build.sh
# ЗАпускаем все необходимые сервисы.
./dc-up-d.sh postgres-redis

# Получаем пароль для пользователя admin
docker compose logs initializer | grep "Admin password:"
