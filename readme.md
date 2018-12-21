# Тестовое задание
Сокращатель URL на Laravel

Фичи:
* Автоматическая генерация
* Возможность самому задать код вместо автоматической генерации
* Возможность задать время жизни короткой ссылки

# Установка
* git clone https://github.com/z-h-z-h/test-feldman-urlshortener.git urlshortener
* composer install
* cp .env.example .env
* Настроить .env - данные MySQL
* php artisan key:generate
* php artisan migrate
* Открываем в браузере
* ??
* Profit!

## Другие варианты реализации сокращателя
Сейчас генерится уникальная строка и проверяется ее отсутствие в БД. Это и есть короткая ссылка.
Можно сделать иначе - создавать запись в БД, получать ID созданной записи и преобразовывать в Base62. Но в БД поле для короткой ссылки все равно придется оставить, чтобы хранить пользовательский вариант короткой ссылки.
