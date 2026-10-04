# 🚀 Gerador e Validador de Quiz Educacional

<div align="center">

[![Status do Projeto](https://img.shields.io/badge/STATUS-EM%20DESENVOLVIMENTO-brightgreen.svg)]()
[![Plataforma](https://img.shields.io/badge/PLATAFORMA-WEB%20%2F%2F%2F%2F%20MOBILE-blue.svg)]()
[![Licença](https://img.shields.io/badge/LICEN%C3%87A-MIT-green.svg)]()
[![Python](https://img.shields.io/badge/PYTHON-3.10%2B-blueviolet.svg)]()
[![React](https://img.shields.io/badge/REACT-18%2B-61DAFB.svg)]()

</div>

---

## 📌 1. Visão Geral do Projeto

O **Gerador e Validador de Quiz Educacional** é uma solução tecnológica avançada desenvolvida sob o ecossistema **ZENTIX** (MGRUPO). O seu principal objetivo é automatizar, gerir e validar o ciclo de vida completo de avaliações pedagógicas, questionários de competências e a respetiva emissão de credenciais/certificados seguros.

A arquitetura do sistema foi concebida para unir robustez corporativa, escalabilidade em nuvem, alto desempenho e total integridade na auditoria de respostas e resultados.

---

## 🏛️ 2. Arquitetura e Stack Tecnológica

O sistema emprega uma arquitetura modular orientada a serviços (Microserviços / Monolito Modular), garantindo o desacoplamento entre as camadas de negócio, interface e persistência:

| Camada do Sistema | Tecnologias / Ferramentas | Descrição e Finalidade |
| :--- | :--- | :--- |
| **Backend & API** | Python (`FastAPI`, `Django REST`), Node.js | Orquestração da lógica de negócio, APIs RESTful assíncronas e motores de pontuação. |
| **Frontend & UI** | React.js, Tailwind CSS, Flutter (Mobile) | Interfaces responsivas, painel administrativo dinâmico e aplicação móvel nativa. |
| **Persistência de Dados** | PostgreSQL (`pgvector`, `PostGIS`), Redis | Base de dados relacional primária, suporte a dados geespaciais e cache de alta performance. |
| **DevOps & Infraestrutura** | Docker, Docker Compose, GitHub Actions | Containerização de ambientes, automação de CI/CD e controlo rigoroso de versões. |

---

## 📂 3. Estrutura de Diretórios do Repositório

O repositório encontra-se organizado de forma a separar claramente a documentação de engenharia, o código-fonte e os manuais operacionais:

```text
gerador-e-validador-de-quiz-educacional/
├── wiki-docs/               # Documentação técnica oficial e DIP do projeto
│   └── DIP-Gerador e Validador de Quiz Educacional.pdf
├── manuais/                 # Manuais de utilização e guias de operação
├── src/                     # Código-fonte principal (Backend, Frontend, Módulos Core)
├── docker-compose.yml       # Orquestração local dos serviços de base de dados e cache
├── .env.example             # Exemplo de variáveis de ambiente do sistema
└── README.md                # Documentação central do repositório
```

---

## ⚙️ 4. Pré-requisitos de Instalação

Antes de proceder com a clonagem e execução do projeto, certifique-se de que possui as seguintes ferramentas configuradas na sua estação de trabalho:
* **Git** (v2.30+)
* **Docker** e **Docker Compose** (recomendado para os serviços de suporte)
* **Python** (v3.10 ou superior)
* **Node.js** (v18.x LTS ou superior) & npm / yarn

---

## 🚀 5. Guia de Instalação e Configuração Local

Siga o procedimento passo a passo abaixo para configurar o ambiente de desenvolvimento:

### 5.1. Clonar o Repositório
```bash
git clone https://github.com/marcio-dev-fullstack/gerador-e-idador-de-quiz-educacional.git
cd gerador-e-idador-de-quiz-educacional
```

### 5.2. Configurar o Ambiente Backend
1. Aceda ao diretório do backend ou raiz do projeto e crie um ambiente virtual Python:
   ```bash
   python -m venv venv
   ```
2. Ative o ambiente virtual:
   * **Windows (PowerShell):** `.\venv\Scripts\Activate`
   * **Linux / macOS:** `source venv/bin/activate`
3. Instale as dependências requeridas:
   ```bash
   pip install -r requirements.txt
   ```

### 5.3. Subir os Serviços de Base de Dados via Docker
Para iniciar instâncias isoladas do PostgreSQL e Redis no seu ambiente local:
```bash
docker-compose up -d
```

---

## 📋 6. Documentação de Engenharia (DIP)

A especificação formal do projeto, premissas arquiteturais, diagramas lógicos e cronogramas encontram-se rigorosamente documentados no Documento de Iniciação do Projeto (DIP):
* 📄 Localização: [`wiki-docs/DIP-Gerador e Validador de Quiz Educacional.pdf`](wiki-docs/DIP-Gerador%20e%20Validador%20de%20Quiz%20Educacional.pdf)

---

## 🤝 7. Contribuição e Licenciamento

* **Padrão de Commit:** Utilize mensagens descritivas seguindo a convenção (`feat:`, `fix:`, `docs:`, `refactor:`).
* **Licença:** Este projeto está licenciado sob os termos da licença **MIT**.

---

## 👨‍💻 Autor e Governança

* **Arquiteto de Software & Desenvolvedor Principal:** Márcio Rodrigues de Oliveira
* **Organização / Ecossistema:** MGRUPO / **ZENTIX** — Projetos & Engenharia