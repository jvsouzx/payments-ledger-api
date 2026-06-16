# Payments Ledger API

API de ledger financeiro desenvolvida para estudar consistência transacional, idempotência, modelagem contábil de dupla entrada e arquitetura backend robusta para sistemas de pagamento.


## Estrutura do Projeto
```
payments-ledger-api/
├── app/
│   ├── __init__.py
│   ├── main.py
│   │
│   ├── core/
│   │   ├── __init__.py
│   │   ├── config.py
│   │   └── database.py
│   │
│   ├── api/
│   │   ├── __init__.py
│   │   └── router.py
│   │
│   ├── modules/
│   │   ├── accounts/
│   │   │   ├── __init__.py
│   │   │   ├── router.py
│   │   │   ├── schemas.py
│   │   │   ├── models.py
│   │   │   └── service.py
│   │   │
│   │   ├── transactions/
│   │   │   ├── __init__.py
│   │   │   ├── router.py
│   │   │   ├── schemas.py
│   │   │   ├── models.py
│   │   │   └── service.py
│   │   │
│   │   └── transfers/
│   │       ├── __init__.py
│   │       ├── router.py
│   │       ├── schemas.py
│   │       └── service.py
│   │
│   └── shared/
│       ├── __init__.py
│       └── exceptions.py
│
├── tests/
│   ├── test_health.py
│   ├── accounts/
│   ├── transactions/
│   └── transfers/
│
├── migrations/
├── pyproject.toml
├── Dockerfile
├── docker-compose.yml
└── README.md
```