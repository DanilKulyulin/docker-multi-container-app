# Настройка Docker Swarm для нескольких сред

Этот проект устанавливает многосредовую настройку Docker Compose для `dev`, `prod` и `lab`. Каждая среда имеет две службы: `web` и `db`.

## Файлы

- **docker-compose.yml**: Общие конфигурации для всех служб.
- **docker-compose.dev.yml**: Переопределения для среды разработки.
- **docker-compose.prod.yml**: Переопределения для производственной среды.
- **docker-compose.lab.yml**: Переопределения для лабораторной среды.

## Использование

### Разработка:

```bash
docker-compose -f docker-compose.yml -f docker-compose.prod.yml up
docker-compose -f docker-compose.yml -f docker-compose.lab.yml up
```
