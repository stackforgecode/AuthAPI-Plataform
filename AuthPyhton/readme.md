# AuthPyhton - API de Autenticação com Django e PostgreSQL

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python Version](https://img.shields.io/badge/Python-3.7%20%7C%203.8%20%7C%203.9-blue)](https://www.python.org/downloads/)
[![Django Version](https://img.shields.io/badge/Django-3.x-green)](https://www.djangoproject.com/)
[![Build Status](https://github.com/stackforgecode/AuthAPI/actions/workflows/build.yml/badge.svg)](https://github.com/stackforgecode/AuthAPI/actions/workflows/build.yml)
[![Coverage Status](https://coveralls.io/repos/github/stackforgecode/AuthAPI/badge.svg?branch=main)](https://coveralls.io/github/stackforgecode/AuthAPI?branch=main)

Este repositório contém uma API de autenticação desenvolvida em Python usando o framework Django e o banco de dados PostgreSQL. A API permite registrar usuários, fazer login e gerar tokens de autenticação usando JWT (JSON Web Tokens).

🏠 [Repositório no GitHub](https://github.com/stackforgecode/AuthAPI)

🔑 **Características principais:**
- Registro de usuários com campos personalizados
- Autenticação de usuários com username e senha
- Geração de tokens JWT para autenticação
- Estrutura de pastas seguindo o padrão DDD (Domain-Driven Design)
- Uso do ORM Django para interação com o banco de dados PostgreSQL
- Testes unitários para garantir o funcionamento correto

## 📁 Estrutura de Pastas e Arquivos
```
AuthAPI/
├── apps/
│   └── authentication/
│       ├── domain/
│       │   ├── models.py
│       │   ├── repositories.py
│       │   ├── services.py
│       │   └── value_objects.py
│       ├── infrastructure/
│       │   ├── __init__.py
│       │   ├── repositories.py
│       │   └── external_services.py
│       ├── migrations/
│       │   ├── __init__.py
│       │   └── ...
│       ├── api/
│       │   ├── serializers.py
│       │   ├── views.py
│       │   ├── urls.py
│       │   └── ...
│       └── tests/
│           ├── __init__.py
│           └── ...
├── config/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── static/
│   └── ...
├── templates/
│   └── ...
├── manage.py
└── requirements.txt
```

## 🚀 Como Executar o Projeto
1. Clone este repositório: `git clone https://github.com/stackforgecode/AuthAPI.git`
2. Navegue para o diretório do projeto: `cd AuthAPI`
3. Instale as dependências: `pip install -r requirements.txt`
4. Configure as informações de conexão do banco de dados no arquivo `settings.py`
5. Execute as migrações do banco de dados: `python manage.py migrate`
6

. Inicie o servidor: `python manage.py runserver`

✅ **Testes Unitários:**
- Execute os testes unitários para garantir o funcionamento correto da API:
  - Navegue para o diretório do projeto: `cd AuthAPI`
  - Execute os testes: `python manage.py test`

## 📝 Licença
Este projeto é licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](https://github.com/stackforgecode/AuthAPI/blob/main/LICENSE) para obter mais informações.

📚 **Referências:**
- [Django Documentation](https://docs.djangoproject.com/)
- [Django REST framework Documentation](https://www.django-rest-framework.org/)
- [Faker Documentation](https://faker.readthedocs.io/)

👤 **Autor:**
- GitHub: [stackforgecode](https://github.com/stackforgecode)

✉️ **Contato:**
Para quaisquer dúvidas ou sugestões, sinta-se à vontade para entrar em contato através do e-mail seuemail@example.com.

Agradeço pelo interesse no projeto e espero que seja útil para suas necessidades de autenticação com Django e PostgreSQL!
