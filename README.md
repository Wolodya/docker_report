# Report page Docker

Обертка для keyua report page project https://github.com/Wolodya/keyua.git
## Getting Started

Для запуска приложения необходимо docker и docker-compose

1. На основе .envs/.django_template .envs/.postgres_template создать файлы .envs/.django .envs/.postgres
2. ```docker-compose build```
3. ```docker-compose up``` или ```docker-compose up -d``` если запускать в демон режиме


### Порты:
- 8000 основной порт на котором весит джанго приложение.

