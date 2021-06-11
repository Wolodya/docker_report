# V2 Report page Docker

Обертка для keyua report page project https://github.com/Wolodya/keyua.git
## Getting Started

Для запуска приложения необходимо docker и docker-compose

1. Склонить проект ```git clone --recurse-submodules https://github.com/Wolodya/docker_report.git```
2. На основе .envs/.django_template .envs/.postgres_template создать файлы .envs/.django .envs/.postgres
3. ```docker-compose build```
4. ```docker-compose up``` или ```docker-compose up -d``` если запускать в демон режиме


### Порты:
- 8000 основной порт на котором джанго приложение.
- 15673 rabbit
- 5555 flower

