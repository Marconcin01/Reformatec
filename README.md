<div align="center">

# 🛠️ Reformatec

**Manutenção e reforma sem dor de cabeça — do primeiro contato ao aceite digital, tudo em uma única conversa.**

[![Deploy](https://img.shields.io/badge/deploy-vercel-black?style=for-the-badge&logo=vercel)](https://reformatec.vercel.app/)
[![Status](https://img.shields.io/website?style=for-the-badge&url=https%3A%2F%2Freformatec.vercel.app)](https://reformatec.vercel.app/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)](#)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](#)
[![jsPDF](https://img.shields.io/badge/jsPDF-2.5.1-red?style=for-the-badge)](#)
[![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)](#)

[**🔗 Acessar a aplicação no ar**](https://reformatec.vercel.app/)

</div>

---

## 📌 Sobre o projeto

**Reformatec** é uma aplicação web front-end que simula um ecossistema completo de captação, orçamento e agendamento para prestadores de serviços residenciais e comerciais (elétrica, hidráulica, pintura e reparos gerais).

O projeto nasceu como um estudo de caso de **landing page orientada à conversão**, evoluindo para um sistema funcional que cobre toda a jornada do cliente: da primeira visita ao site, passando pela geração de um orçamento personalizado com valores reais, até o aceite digital e o agendamento do serviço — sem sair do WhatsApp.

Todo o sistema roda **100% no navegador** (sem backend ou banco de dados), usando `localStorage`/`sessionStorage` para persistência local e a API de URL do WhatsApp e do Google Calendar para integrações externas — uma demonstração de até onde é possível levar uma stack front-end simples quando bem arquitetada.

---

## ✨ Principais funcionalidades

- 🧮 **Orçamento dinâmico em cascata** — seleção de categoria → serviço específico, com precificação automática e cálculo do total em tempo real.
- 📄 **Exportação em PDF** — geração de uma fatura profissional (cabeçalho de marca, tabela de itens, total em destaque) via [`jsPDF`](https://github.com/parallax/jsPDF), com download automático.
- 💬 **Integração com WhatsApp** — mensagens pré-formatadas e automatizadas para envio do orçamento, aceite digital e confirmação de agendamento, via links `wa.me`.
- 📅 **Sincronização com Google Calendar** — geração de link parametrizado (`calendar.google.com/calendar/render`) que cria o evento de agendamento já preenchido (data, horário e descrição).
- 🔐 **Painel administrativo protegido** — dashboard interno com autenticação simples (login/senha) e métricas em tempo real (total de orçamentos, aprovados e faturamento potencial), com dados persistidos via `localStorage`.
- 🖼️ **Galeria "Antes e Depois"** — seção de cases reais exibindo o resultado de projetos concluídos.
- 🌓 **Design Dark Mode + Glassmorphism** — interface moderna construída com Tailwind CSS, efeitos de vidro fosco (`backdrop-blur`), gradientes e microinterações.

---

## 🧱 Tecnologias empregadas

| Tecnologia | Uso no projeto |
|---|---|
| **HTML5** | Estrutura semântica de toda a aplicação |
| **Tailwind CSS** (via CDN) | Estilização utilitária, tema Dark Mode e Glassmorphism |
| **JavaScript (Vanilla)** | Toda a lógica de interatividade, formulários em cascata, autenticação e persistência |
| **jsPDF** | Geração client-side do PDF do orçamento |
| **Font Awesome** | Iconografia |
| **Google Fonts** (Plus Jakarta Sans + Inter) | Tipografia |
| **Vercel** | Hospedagem e deploy contínuo via GitHub |

> Projeto construído sem frameworks, bundlers ou etapas de build — um único arquivo `index.html`, pronto para rodar em qualquer lugar.

---

## 🚀 Como acessar / testar

### Aplicação no ar

🔗 **[https://reformatec.vercel.app/](https://reformatec.vercel.app/)**

### Rodando localmente

Por não depender de build, basta um navegador:

```bash
# 1. Clone o repositório
git clone https://github.com/seu-usuario/reformatec.git

# 2. Entre na pasta do projeto
cd reformatec

# 3. Abra o index.html no navegador
# (duplo clique no arquivo, ou use uma extensão como Live Server no VS Code)
```

Não há dependências para instalar nem variáveis de ambiente — todos os recursos externos (Tailwind, Font Awesome, Google Fonts, jsPDF) são carregados via CDN.

### Fluxo sugerido para teste

1. Preencha o formulário na seção **"Sistema"** para gerar um orçamento (baixa um PDF e abre o WhatsApp).
2. Copie o link de aceite gerado (`?aceite=NUMERO`) e abra em uma nova aba para simular a jornada do cliente.
3. Escolha data e horário e confirme o agendamento (abre o WhatsApp e o Google Calendar).
4. Acesse o **Painel Administrativo** pelo botão no topo do site — usuário `admin`, senha `reformatec2026` — para ver os orçamentos registrados.

> ⚠️ O painel administrativo é uma simulação para fins de portfólio: a autenticação roda inteiramente no navegador, então não deve ser usada como proteção real de dados sensíveis.

---

## 👨‍💻 Autor

Desenvolvido por **Renan Marconcin Almeida**.

<div align="left">

<!-- Sugestão: adicione seus links de contato/portfólio abaixo -->
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](#)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](#)

</div>

---

<div align="center">

*Reformatec é um projeto fictício, criado para fins de estudo e demonstração de portfólio.*

</div>
