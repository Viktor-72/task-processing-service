# Task Processing Service
HTTP-сервис для создания и обработки задач.

## 🔧 Запуск
Сервер запускается на порту `8080`.

### 📦 Требования
- Go 1.23+

### 🚀 Быстрый старт
```bash
go run ./cmd/app
```

_____________________________________________________________________
### Конфигурация
Файл конфигурации: configs/server.cfg.yaml


# OpenApi (генерация HTTP сервера)
```
oapi-codegen -config configs/server.cfg.yaml api/openapi/openapi.yml
```

# Документация используемых библилиотек
* [Oapi-codegen] (https://github.com/oapi-codegen/oapi-codegen)

_____________________________________________________________________


### Структура проекта
cmd/app — точка входа в приложение
internal/ — бизнес-логика, адаптеры, порты
api/openapi/ — OpenAPI спецификация
configs/ — YAML конфигурация
generated/servers.gen.go — сгенерированные типы и интерфейсы