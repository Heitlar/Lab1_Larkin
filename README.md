### Архитектурная диаграмма пакетов проекта (Многослойная архитектура)

```mermaid
subgraph "forum_project (Application)"
    api[...] --> bll[...]
    bll[...] --> dal[...]
end

db[(База данных)]

api --> |Presentation| Клиент/Фронтенд
dal --> |SQL / ORM| db

style api fill:#f9f,stroke:#333,stroke-width:2px
style bll fill:#bbf,stroke:#333,stroke-width:2px
style dal fill:#fbf,stroke:#333,stroke-width:2px
style db fill:#f96,stroke:#333,stroke-width:2px
```
