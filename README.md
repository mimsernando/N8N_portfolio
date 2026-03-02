# Portfólio de Automações com n8n

## Sobre o Projeto

Este repositório é uma demonstração prática das minhas habilidades em automação e integração de sistemas utilizando n8n. O projeto foi desenvolvido para explorar e aplicar os conceitos basicos do N8N, como a criação de agentes de IA, integração via API e organização de dados.

O sistema central é um agente de atendimento para WhatsApp, projetado de forma modular e escalável.

**Status do Projeto:** Em desenvolvimento contínuo.

---

## Workflow Principal: Agente de Atendimento com IA

Desenvolvi um fluxo principal em n8n que simula uma secretária virtual para uma clínica. O sistema é acionado por um **Webhook** de uma **API de WhatsApp** e orquestra todo o processo de atendimento.

### Funcionalidades e Conceitos Aplicados:

*   **Criação de Agente de IA:** O núcleo do sistema é um agente de IA construído com a API da **OpenAI**. O prompt foi cuidadosamente elaborado para definir a persona, as regras de negócio e as ferramentas que o agente pode usar, como consultar a agenda.

*   **Integração de Sistemas via API:**
    *   **Webhook/REST API:** O fluxo recebe e envia dados para a Evolution API.
    *   **Google Calendar API:** O agente se conecta à agenda para verificar disponibilidade e realizar agendamentos, demonstrando a integração com serviços de terceiros.
    *   **Redis:** Utilizado para cache e gerenciamento de estado da conversa, uma prática comum em sistemas de automação.

*   **Organização de Dados:**
    *   O fluxo normaliza os dados brutos recebidos do webhook para um formato estruturado e consistente.
    *   Os fluxos auxiliares demonstram a consulta em um banco de dados **Supabase/Postgres** para recuperar informações de agendamentos, mostrando a noção de organização de dados relacionais.

*   **Estrutura Modular:** O sistema foi dividido em um fluxo principal (orquestrador) e fluxos auxiliares (sub-rotinas para tarefas como "buscar evento" ou "verificar disponibilidade"), o que facilita a manutenção e o teste.

---

## Ferramentas e Tecnologias

*   **n8n:** Plataforma central para a criação e ajuste dos fluxos.
*   **OpenAI:** Criação do agente de IA.
*   **API REST / Webhooks:** Principal método de integração.
*   **Supabase / Postgres:** Noções de organização de dados.
*   **Redis:** Gerenciamento de estado.
*   **Google Calendar API:** Integração com sistemas externos.

---

## Autor

**Fernando Simola Ferrandis**
