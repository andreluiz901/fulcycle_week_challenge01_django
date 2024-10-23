# 📝 Meu Blog - My Blog - Challenge1

Bem-vindo ao Meu Blog! Este é um projeto simples de blog desenvolvido com Django, onde você pode listar e visualizar postagens. O blog foi criado para praticar o uso do Django e compreender a estrutura de um aplicativo web durante a semana Full Cycle.

## 🚀 Tecnologias Usadas

- **Python**: Linguagem de programação usada para desenvolver o projeto.
- **Django**: Framework web que facilita a construção de aplicações web robustas.
- **SQLite**: Banco de dados leve e integrado que armazena os dados do blog.
- **HTML/CSS**: Estrutura e estilo das páginas do blog.
- **Git**: Controle de versão utilizado para gerenciar o código-fonte.

## 📦 Instalação

### Pré-requisitos

Certifique-se de ter o Python e o Pipenv instalados em seu sistema. Você pode verificar isso executando os seguintes comandos:

```bash
python --version
pipenv --version
```

## Passos para Rodar o Projeto Localmente

### 1. Clone o repositório

Use o comando abaixo para clonar o repositório em sua máquina:

`git clone <URL_DO_REPOSITORIO>`

Navegue até o diretório do projeto:

`cd nome_do_repositorio`

### 2. Crie um ambiente virtual

Crie um ambiente virtual com o Pipenv:

`pipenv install`

### 3. Ative o ambiente virtual

Ative o ambiente virtual com o seguinte comando:

`pipenv shell`

### 4. Migrate do Banco de Dados

Após ativar o ambiente, execute as migrações para criar as tabelas do banco de dados:

`python manage.py migrate`

### 5. Crie um Superusuário (opcional)

Se você quiser acessar o painel de administração do Django, crie um superusuário com o comando:

`python manage.py createsuperuser`

Siga as instruções na tela para criar suas credenciais.

### 6. Execute o Servidor

`python manage.py runserver`

### 7. Acesse o Blog

Abra seu navegador e acesse http://127.0.0.1:8000/ para ver a lista de postagens do blog. Para acessar o painel de administração, vá para http://127.0.0.1:8000/admin e faça login com o superusuário que você criou.

Por lá você pode cadastrar novos posts e novas tags.

## 🖼️ Estrutura do Projeto

```bash
nome_do_repositorio/
│
├── .venv/                       # Controle do ambiente virtual e dependências
├── core/                       # Aplicativo principal do blog
│   ├── migrations/             # Arquivos de migração do banco de dados
│   ├── static/             # Arquivos estáticos de views do projeto
│   ├── templates/              # Templates HTML do Django
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py               # Modelos do Django
│   ├── tests.py
│   ├── urls.py                 # URLs do aplicativo
│   └── views.py                # Views do aplicativo
│
├── myblog/                       # Aplicativo inicial do blog
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py               # Modelos do Django
│   ├── tests.py
│   ├── urls.py                 # URLs do aplicativo
│   └── views.py                # Views do aplicativo
│
├── manage.py                   # Script de gerenciamento do Django
├── Pipfile                     # Dependências do projeto
├── Pipfile.lock                # Bloqueio de versões de dependências
└── db.sqlite3            # Arquivo de db sqlite do projeto
```

## 📄 Contribuições

Sinta-se à vontade para contribuir com melhorias e correções. Basta abrir um pull request ou issue.

## 🙌 Agradecimentos

Obrigado por conferir o Meu Blog! E obrigado especial ao time do FUll Cycle com aulas incríveis de diversas linguagens e tecnologias.
