# 🚀 CodingAsOne • Node.js Boilerplate

**Boilerplate oficial da organização [CodingAsOne](https://github.com/CodingAsOne)**  
Base profissional para desenvolvimento de APIs e microsserviços em Node.js + TypeScript.

> 🧱 Este repositório é o ponto de partida para todos os projetos da Codehouse **CodingAsOne**, garantindo padronização, escalabilidade e boas práticas de engenharia de software.

---

## 🧭 Sobre a CodingAsOne

A **CodingAsOne** é uma Codehouse que oferece soluções completas em desenvolvimento de software — da concepção à entrega.

Nosso propósito é **unir pessoas, processos e tecnologia**, criando sistemas consistentes, escaláveis e fáceis de manter.

> “Criamos código com propósito, como um só time.”

---

## 🧩 Stack do Boilerplate

| Área | Ferramenta | Descrição |
|------|-------------|-----------|
| 🧠 Linguagem | **TypeScript** | Base tipada para melhor manutenção |
| ⚙️ Framework | **Express.js** | Estrutura leve e flexível para APIs |
| 🗄️ ORM | **TypeORM** | Mapeamento de entidades e migrations |
| 🔐 Auth | **JWT + dotenv** | Autenticação e variáveis de ambiente |
| 📘 Docs | **Swagger** | Especificação de endpoints (`api-spec.yaml`) |
| 🧪 Testes | **Jest** | Testes unitários e de integração |
| 🧹 Lint | **ESLint + Prettier** | Padrões e formatação de código |
| 🐳 Infra | **Docker + docker-compose** | Containerização e ambiente padronizado |
| 🔄 CI/CD | **GitHub Actions** | Pipeline automatizada |
| 🧠 Qualidade | **SonarQube (opcional)** | Métricas e análise estática |
| 📈 Observabilidade | **New Relic (opcional)** | Monitoramento de performance |

---

## 🧱 Estrutura do Projeto

```bash
src/
 ├── config/          # Configurações de ambiente, banco, etc.
 ├── controllers/     # Camada de controle (rotas)
 ├── services/        # Regras de negócio
 ├── repositories/    # Acesso a dados
 ├── models/          # Entidades TypeORM
 ├── middlewares/     # Middlewares globais
 ├── routes/          # Rotas da aplicação
 ├── utils/           # Funções utilitárias
 ├── dependencies.ts  # Registro de dependências (typedi)
 └── app.ts           # Ponto de entrada da aplicação
tests/
 ├── controllers/
 └── services/
```
⚙️ Scripts
Comando	Descrição
```bash
npm run dev	Inicia o servidor com hot reload (ts-node-dev)
npm run build	Compila o projeto para /build
npm start	Executa o build em produção
npm run test	Roda os testes com cobertura
npm run lint	Verifica padrões de código
npm run lint:fix	Corrige erros de lint automaticamente
npm run migration	Executa migrations compiladas
npm run migration:create	Cria nova migration
npm run migration:revert	Reverte última migration
```
🔐 Variáveis de Ambiente (.env)
```env
PORT=3000
JWT_SECRET=changeme_secret

TYPEORM_CONNECTION=postgres
TYPEORM_DATABASE=mydb
TYPEORM_HOST=localhost
TYPEORM_PORT=5432
TYPEORM_USERNAME=user
TYPEORM_PASSWORD=pass
TYPEORM_SYNCHRONIZE=false
TYPEORM_ENTITIES=build/src/models/*.js
TYPEORM_MIGRATIONS=build/migrations/*.js
TYPEORM_LOGGING=true

NON_CORPORATE_EMAIL_CLIENTS="@gmail,@hotmail,@yahoo,@outlook,@uol"
```
## 🧠 Estrutura Organizacional • CodingAsOne
A CodingAsOne é formada por times multifuncionais, que colaboram entre si para entregar soluções de ponta, de forma ágil e padronizada.

🧑‍💻 Development Team
Responsável pelo desenvolvimento técnico dos sistemas, APIs e integrações.

| Cargo                   | Descrição                                                  |
| ----------------------- | ---------------------------------------------------------- |
| **Tech Lead**           | Define padrões técnicos e orienta o time                   |
| **Backend Developer**   | Implementa lógica de negócio, integrações e banco de dados |
| **Frontend Developer**  | Desenvolve interfaces e integra com APIs                   |
| **Fullstack Developer** | Atua nas duas frentes, garantindo integração ponta a ponta |
| **Mobile Developer**    | Responsável por apps híbridos ou nativos                   |
| **DevOps Engineer**     | Cuida da automação, CI/CD e infraestrutura em nuvem        |


🧩 QA & Quality Team
Garante a qualidade e estabilidade das entregas através de testes e validações.

| Cargo                   | Descrição                                       |
| ----------------------- | ----------------------------------------------- |
| **QA Lead**             | Planeja estratégias de testes e automação       |
| **QA Analyst**          | Executa testes manuais e automatizados          |
| **Automation Engineer** | Cria e mantém pipelines de testes automatizados |

🧭 Product & UX Team
Central de planejamento e experiência do usuário.

| Cargo                | Descrição                                             |
| -------------------- | ----------------------------------------------------- |
| **Product Owner**    | Define prioridades e escopo de produto                |
| **UX/UI Designer**   | Cria fluxos e interfaces centradas no usuário         |
| **Business Analyst** | Traduz necessidades de negócio em requisitos técnicos |

🧱 Support & Operations

| Cargo                          | Descrição                                           |
| ------------------------------ | --------------------------------------------------- |
| **Scrum Master / Agile Coach** | Garante ritmo e boas práticas ágeis                 |
| **Infra Engineer**             | Gerencia servidores, monitoramento e escalabilidade |
| **Client Manager**             | Faz a ponte entre cliente e equipe técnica          |


💼 Estrutura Interna da Organização no GitHub
| Team         | Descrição                                 | Acesso           |
| ------------ | ----------------------------------------- | ---------------- |
| `Developers` | Desenvolvedores principais da organização | Push/PR          |
| `QA`         | Analistas e testadores de qualidade       | PR e revisão     |
| `DevOps`     | Automação, pipelines e Docker             | Deploy/CI        |
| `Managers`   | Gerentes e Product Owners                 | Leitura total    |
| `Clients`    | Acesso a projetos dedicados               | Leitura restrita |


##### Cada time possui permissões específicas dentro da organização CodingAsOne, garantindo segurança e rastreabilidade em cada repositório.
---
## 🌍 Uso do Template
Vá até o repositório boilerplate-node

Clique em "Use this template"

Escolha o nome do novo repositório

Ajuste o .env e rode:

```bash
npm install
npm run dev
```
---
🧭 Próximos Passos

👩‍💻 Para continuar sua jornada dentro do ecossistema CodingAsOne, siga para o repositório de tutoriais e guias internos.

📘 Acesse o repositório de tutoriais:
👉 CodingAsOne / tutorials

Lá você encontrará:

📦 Como configurar CI/CD no GitHub Actions

🔄 Padrão de registro no dependencies.ts

🧪 Guia de testes unitários e mocks

🧰 Padronização de commits e versionamento

☁️ Deploy automatizado com AWS e Docker Compose

💡 Dicas e boas práticas internas de desenvolvimento
---
🧾 Licença
> Licenciado sob a MIT License
© 2025 — CodingAsOne

✨ "We build. We learn. We grow. — CodingAsOne"
