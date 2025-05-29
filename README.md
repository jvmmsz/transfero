🎬 StreamVibe
![Tela Login Site](https://github.com/user-attachments/assets/0211c202-6882-411f-8f2e-720e6b326f24)
![Tela do Site](https://github.com/user-attachments/assets/1d1f5679-f28f-4525-b5cf-defa744b273c)
 - Plataforma de Streaming de Filmes 🍿
Este é um projeto web desenvolvido com Django 🐍 que simula uma plataforma de streaming de filmes. O sistema permite gerenciar usuários 👤, exibir catálogos 🎞️ e organizar conteúdos de forma escalável e modular 🧩.

🚀 Funcionalidades
✅ Cadastro e gerenciamento de usuários 👥

🎥 Catálogo de filmes com visualização por templates

♻️ Estrutura modular com reaproveitamento de componentes globais

🖼️ Gerenciamento de mídias (imagens, vídeos etc.)

🎨 Estilo e templates organizados de forma reutilizável

🗂 Estrutura de Diretórios 📁
php
Copiar
Editar
├── transfero/               # 📌 Diretório principal do projeto Django
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py          # ⚙️ Configurações do projeto
│   ├── urls.py ![Urls py](https://github.com/user-attachments/assets/4f25f1c1-8bb0-4034-9ee3-b257bb163bd5) # 🌐 Roteamento principal
│   └── wsgi.py ![Wsgi py](https://github.com/user-attachments/assets/5708ca20-abe3-4336-9ca9-7158a0b621ab)


├── usuarios/                # 👤 App para gestão de usuários
│   ├── admin.py 
│   ├── apps.py
│   ├── models.py
│   ├── tests.py
│   └── urls.py

├── filmes/                  # 🎬 App principal do streaming
│   ├── admin.py
│   ├── apps.py ![Apps py](https://github.com/user-attachments/assets/8ea30fa6-ff9e-475a-914a-4294899afd95)
│   ├── forms.py ![Forms py](https://github.com/user-attachments/assets/97b917f4-09a1-439e-93cf-e2731afab21a)
│   ├── models.py
│   ├── views.py ![Views py](https://github.com/user-attachments/assets/1f1d6dab-e720-4415-af4c-b0e2e4afcbb6)
│   ├── urls.py ![Urls py](https://github.com/user-attachments/assets/53f513d1-efdd-4176-b68c-310fa9dfdb5a)
│   └── templates/
│       └── filmes/          # 🧾 Templates específicos dos filmes

├── sistema/                 # 🧠 App auxiliar do sistema
│   ├── migrations/
│   ├── templates/
│   └── views/

├── base_templates/           ![Base ](https://github.com/user-attachments/assets/2af681c9-5f0d-475d-9808-94537ae8530b)

│   └── global/
│       └── partials/        # 🧩 Ex: navbar, footer, etc.

├── base_static/             # 🎨 Arquivos estáticos globais
│   └── global/
│       ├── assets/
│       └── css/

├── static/                  # 📂 Staticfiles (coleta final)
├── media/                   # 🖼️ Uploads de imagens ou vídeos
├── imagens/                 # 🖼️ Diretório auxiliar para imagens
├── venv/                    # 🐍 Ambiente virtual
├── anotacoes.md             # 📝 Notas e anotações do projeto
├── db.sqlite3               # 🗃️ Banco de dados SQLite
└── manage.py                # 🛠️ Arquivo principal para comandos Django
⚙️ Como rodar o projeto 💻
bash
Copiar
Editar
# 📥 Clone o repositório
git clone https://github.com/seu-usuario/transfero.git
cd transfero

# 🔁 Ative o ambiente virtual
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows

# 📦 Instale as dependências
pip install -r requirements.txt

# 🔧 Execute as migrações
python manage.py migrate

# ▶️ Rode o servidor
python manage.py runserver
📸 Telas e Layout 🎨
O projeto utiliza uma organização clara de templates 🧾 e estáticos 🎨 para fácil manutenção e personalização. Componentes como header, footer e navbar estão centralizados em base_templates/global/partials.
