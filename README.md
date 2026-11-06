# BarberiaMax - Sistema de Agendamento de Barbearia

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

O **BarberiaMax** é uma solução web desenvolvida para otimizar a gestão de horários e serviços em barbearias de pequeno e médio porte. O sistema busca resolver problemas recorrentes na rotina de agendamento, como acúmulo de faltas de clientes (absenteísmo), falhas na comunicação de confirmação e a ineficiência do agendamento manual via telefone, WhatsApp ou planilhas.

Com o objetivo geral de digitalizar e simplificar a relação entre a barbearia, os barbeiros e os clientes, a plataforma permite a marcação online autônoma de horários 24/7, a gestão unificada da agenda dos profissionais e o envio automatizado de lembretes, proporcionando maior eficiência operacional e melhor experiência ao usuário.

---

## Equipe (Autores)

- **Aluno A** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)
- **Aluno B** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)
- **Aluno C** - [GitHub](https://github.com) | [LinkedIn](https://linkedin.com)

**Orientador(a):** Prof. Nome do Orientador

---

## Funcionalidades Principais

- [x] **Autenticação e Perfis de Acesso:** Acesso diferenciado para Administrador, Recepcionista, Barbeiro e Cliente.
- [x] **Agendamento Online de Serviços:** Escolha de serviço (corte, barba, pigmentação, química, etc.), profissional (barbeiro), data e horário disponível.
- [x] **Gestão da Agenda do Barbeiro:** Painel para o profissional visualizar os cortes diários, alterar status (concluído, cancelado, na cadeira) e definir horários de atendimento/folgas e pausas para almoço.
- [x] **Confirmação e Lembretes:** Notificações automáticas via e-mail e/ou WhatsApp para confirmação prévia do agendamento.
- [x] **Histórico e Preferências do Cliente:** Registro do histórico de serviços realizados e anotações sobre preferências (ex: numeração do pente, estilo de corte).
- [x] **Módulo de Relatórios e Métricas:** Gráficos de absenteísmo, serviços mais procurados, desempenho por barbeiro e volume de atendimentos mensais.

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
$ git clone [https://github.com/usuario/barberiamax.git](https://github.com/usuario/barberiamax.git)

# 2. Acesse a pasta do projeto
$ cd barberiamax

# 3. Instale as dependências do back-end e front-end
$ npm install
# ou
$cd backend && npm install$ cd ../frontend && npm install

# 4. Configure o arquivo de variáveis de ambiente (.env)
# Crie um arquivo .env na raiz/backend seguindo o exemplo do .env.example
# Defina as credenciais do banco de dados e chaves de envio de e-mail

# 5. Execute as migrações e popule o banco de dados
$npm run db:migrate$ npm run db:seed

# 6. Inicie a aplicação
$ npm run dev
