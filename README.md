# 📋 Laboratório: Aplicação Web de Gestão de Tarefas  
## 🎯 Objetivo  
Desenvolver uma aplicação web full-stack para gerenciamento de tarefas, aplicando boas práticas de qualidade de software, acessibilidade, segurança e privacidade.  

  
## 🛠️ Tecnologias Utilizadas
- Backend: Python, Flask, SQLAlchemy, PostgreSQL

- Frontend: HTML5, CSS3, JavaScript

- Ferramentas: VSCode, Git/GitHub, Node.js/npm

- Testes: pytest
  
  
## 📁 Estrutura do Projeto
text  
lab_todolist/  
  ├── app.py              # Aplicação Flask principal  
  ├── requirements.txt    # Dependências Python  
  ├── test_app.py        # Testes automatizados  
  ├── templates/         # Templates HTML  
  ├── static/           # Arquivos estáticos (CSS)  
  ├── venv/             # Ambiente virtual Python  
  └── .gitignore        # Arquivos ignorados pelo Git  
  
  
## ✅ Funcionalidades Implementadas  
✅ CRUD completo de tarefas (Criar, Ler, Atualizar, Deletar)

✅ Interface acessível (WCAG 2.2)

✅ Proteção contra injeção SQL (OWASP)

✅ Validação de dados no backend

✅ Testes unitários e de integração

✅ Versionamento com Git/GitHub
  
  
## 🔒 Conformidade Normativa
WCAG 2.2: Contraste adequado, navegação por teclado, HTML semântico

OWASP Top 10: Prevenção contra injeção SQL, controle de acesso

LGPD: Minimização de dados, direito de exclusão

ISO/IEC 25010: Manutenibilidade, confiabilidade, adequação funcional
  
  
## 🚀 Como Executar
#### 1. Configuração do Ambiente
bash
#Clonar repositório
git clone https://github.com/seu-usuario/lab-flask-acessivel.git
cd lab-flask-acessivel
  
#Criar ambiente virtual
python -m venv venv
source venv/bin/activate  # Linux/Mac
'#' ou .\venv\Scripts\activate  # Windows
  
#Instalar dependências
pip install -r requirements.txt
#### 2. Configurar Banco de Dados
sql
-- Criar usuário e banco no PostgreSQL
CREATE USER dev_user WITH PASSWORD 'dev_pass';
CREATE DATABASE todolist_db OWNER dev_user;
  
#### 3. Executar Aplicação
bash
#Criar tabelas
python -c "from app import app, db; with app.app_context(): db.create_all()"
  
#Iniciar servidor
python app.py
Acesse: http://localhost:5000
  
#### 4. Executar Testes
bash
pytest test_app.py

Commits descritivos no Git

Conformidade com PEP 8 (Python)
