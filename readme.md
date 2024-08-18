📋 Projeto: Assistente de Personal Trainer Automatizado
Este repositório contém o código e as instruções para o desenvolvimento de um Assistente de Personal Trainer Automatizado, utilizando técnicas avançadas de Prompt Engineering. O objetivo deste projeto é criar um prompt que ajude a montar o treino ideal para cada combinação de fatores, como biotipo corporal, disponibilidade de tempo e tipo de exercícios preferidos, proporcionando uma experiência de personalização única para os usuários.

🛠️ Tecnologias Utilizadas
Python: Linguagem principal para o desenvolvimento do prompt e lógica de personalização.
GPT-3.5/GPT-4: Modelo de linguagem utilizado para gerar prompts e adaptar o treino ao perfil do usuário.
Streamlit: Framework utilizado para criar uma interface de usuário interativa e amigável.
Docker: Para containerização e fácil deploy do projeto.
GitHub Actions: Para CI/CD, garantindo que o código seja testado e implantado automaticamente.

🗂️ Estrutura de Diretórios
prompt-challenger-personal-ia/
│
├── .github/
│   └── workflows/   # Configurações para CI/CD
│
├── data/            # Diretório para dados de exemplo ou datasets relevantes
│   ├── example_users.json
│   └── ...
│
├── notebooks/       # Jupyter Notebooks para desenvolvimento e experimentação
│   ├── prompt-engineering.ipynb
│   └── ...
│
├── src/             # Código-fonte do projeto
│   ├── prompts/     # Prompt templates e lógica de criação
│   │   ├── generate_prompt.py
│   │   └── ...
│   ├── app.py       # Código principal do aplicativo Streamlit
│   └── ...
│
├── tests/           # Testes automatizados
│   ├── test_prompts.py
│   └── ...
│
├── Dockerfile       # Dockerfile para containerização
├── requirements.txt # Dependências do projeto
└── README.md        # Documentação principal do projeto

🚀 Instruções de Instalação
Clone o Repositório:
git clone https://github.com/digitalinnovationone/prompt-challenger-personal-ia.git
cd prompt-challenger-personal-ia

Crie um ambiente virtual e ative-o:
python -m venv venv
source venv/bin/activate  # No Windows use `venv\Scripts\activate`

Instale as dependências:
pip install -r requirements.txt

Execute o Aplicativo:
streamlit run src/app.py

🧪 Testes
Execute os testes automatizados para garantir que tudo está funcionando corretamente:
pytest tests/

📦 Docker
Para rodar o projeto em um container Docker:

Build o Docker container:
docker build -t personal-trainer-ia .

Execute o container:
docker run -p 8501:8501 personal-trainer-ia

Agora, você pode acessar o aplicativo em http://localhost:8501.

📄 Licença
Este projeto é licenciado sob a MIT License.
