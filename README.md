# HealthSched - Sistema de Agendamento Médico

> **Projeto de Conclusão de Curso (TCC)** apresentado ao Curso Técnico em Desenvolvimento de Sistemas como requisito parcial para obtenção do título de Técnico em Desenvolvimento de Sistemas.

## Sumário

- [Sobre o Projeto](#-sobre-o-projeto)
- [Equipe (Autores)](#-equipe-autores)
- [Funcionalidades Principais](#-funcionalidades-principais)
- [Tecnologias Utilizadas](#-tecnologias-utilizadas)
- [Arquitetura e Modelagem](#-arquitetura-e-modelagem)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Documentação do TCC](#-documentação-do-tcc)

---

## Sobre o Projeto

O **HealthSched** é uma solução web desenvolvida para otimizar a gestão de consultas e horários em clínicas médicas de pequeno e médio porte. O sistema busca resolver problemas recorrentes na rotina de agendamento, como acúmulo de faltas de pacientes (absenteísmo), falhas na comunicação de confirmação e a ineficiência do agendamento manual via telefone ou planilhas.

Com o objetivo geral de digitalizar e simplificar a relação entre clínica, médicos e pacientes, a plataforma permite a marcação online autônoma de consultas 24/7, a gestão unificada da agenda dos profissionais de saúde e o envio automatizado de lembretes, proporcionando maior eficiência operacional e melhor experiência ao usuário.

---

## Equipe (Autores)

- **Aluno A** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)
- **Aluno B** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)
- **Aluno C** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)

**Orientador(a):** Prof. Nome do Orientador

---

## Funcionalidades Principais

- [x] **Autenticação e Perfis de Acesso:** Acesso diferenciado para Administrador, Recepcionista, Médico e Paciente.
- [x] **Agendamento Online de Consultas:** Escolha de especialidade médica, profissional, data e horário disponível.
- [x] **Gestão da Agenda Médica:** Painel para o profissional visualizar consultas diárias, alterar status (atendido, cancelado, em espera) e definir horários de atendimento/folgas.
- [x] **Confirmação e Lembretes:** Notificações automáticas via e-mail e/ou WhatsApp para confirmação prévia da consulta.
- [x] **Prontuário/Histórico do Paciente:** Registro simples do histórico de consultas e observações técnicas da consulta.
- [x] **Módulo de Relatórios e Métricas:** Gráficos de absenteísmo, especialidades mais procuradas e volume de atendimentos mensais.

---

## Tecnologias Utilizadas

- **Front-end:** HTML5, CSS3, JavaScript, React.js (com Styled Components/Tailwind CSS).
- **Back-end:** Node.js (Express) / Python (FastAPI/Django) / PHP (Laravel).
- **Banco de Dados:** PostgreSQL / MySQL.
- **Serviços Externos:** Nodemailer (Envio de e-mails) e Twilio/WhatsApp API (Lembretes).
- **Ferramentas e Design:** Figma (Prototipagem UI/UX), Git, GitHub, Postman.

---

## Arquitetura e Modelagem

- **Modelo Entidade-Relacionamento (MER):** ![Diagrama MER](./docs/diagrama_mer.png)
- **Diagrama de Casos de Uso:** ![Diagrama Casos de Uso](./docs/casos_de_uso.png)
- **Diagrama de Classe:** ![Diagrama de Classe](./docs/diagrama_classes.png)

---

## Como Executar o Projeto

### Pré-requisitos

Antes de começar, certifique-se de ter instalado em sua máquina:

- [Git](https://git-scm.com)
- [Node.js](https://nodejs.org) (v18 ou superior)
- Banco de Dados [PostgreSQL](https://www.postgresql.org/) ou [MySQL](https://mysql.com)

### Passo a Passo

```bash
# 1. Clone este repositório
$ git clone https://github.com/usuario/healthsched.git

# 2. Acesse a pasta do projeto
$ cd healthsched

# 3. Instale as dependências do back-end e front-end
$ npm install
# ou
$ cd backend && npm install
$ cd ../frontend && npm install

# 4. Configure o arquivo de variáveis de ambiente (.env)
# Crie um arquivo .env na raiz/backend seguindo o exemplo do .env.example
# Defina as credenciais do banco de dados e chaves de envio de e-mail

# 5. Execute as migrações e popule o banco de dados
$ npm run db:migrate
$ npm run db:seed

# 6. Inicie a aplicação
$ npm run dev
```

O servidor local iniciará na porta `:3000` (Front-end) e `:5000` (Back-end API). 
Acesse: <http://localhost:3000>

---

## Documentação do TCC

Acesse a documentação acadêmica do projeto nos links abaixo:

- [Monografia Completa (PDF)](./docs/monografia_tcc.pdf)
- [Slides da Apresentação da Banca (PDF)](./docs/slides_apresentacao.pdf)
- [Manual do Usuário (PDF)](./docs/manual_usuario.pdf)
