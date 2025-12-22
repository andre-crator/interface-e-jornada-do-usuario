# Arquitetura da Informação (IA)

## Objetivo

Definir a estrutura de conteúdo e navegação do sistema de controle de estudos, garantindo que o usuário
consiga realizar as tarefas principais de forma simples, rápida e sem confusão.

Esta arquitetura foi construída com base em:
- Persona 01 (estudante universitário)
- Problema do usuário (falta de organização e visão de progresso)
- Jornada do usuário (login → cadastro de matérias → atualização de progresso → visualização)

---

## Principais Conteúdos do Sistema

O sistema precisa oferecer ao usuário:

- Autenticação (Login)
- Lista de matérias cadastradas
- Cadastro de nova matéria
- Atualização de progresso de uma matéria
- Visualização clara de progresso (percentual/status)
- Acesso rápido ao contato/suporte (opcional)

---

## Mapa do Site (Sitemap)
[Login] | v [Home / Dashboard] ├── [Matérias] │     ├── [Listar Matérias] │     ├── [Cadastrar Matéria] │     └── [Detalhe da Matéria] │            └── [Atualizar Progresso] | └── [Perfil / Conta] (opcional)

---

## Descrição das Telas

### 1) Tela de Login
*Objetivo:* permitir acesso ao sistema  
*Campos:* e-mail, senha  
*Ações:* entrar, recuperar senha (opcional)

---

### 2) Home / Dashboard
*Objetivo:* visão geral rápida do progresso do usuário  
*Exibe:*
- resumo de matérias (quantidade total)
- matérias em andamento
- matérias concluídas
- atalho para “Cadastrar Matéria”

---

### 3) Tela de Matérias (Listagem)
*Objetivo:* mostrar todas as matérias cadastradas  
*Exibe:*
- nome da matéria
- status (ex: em andamento / concluída)
- percentual de progresso
*Ações:*
- abrir detalhe
- cadastrar nova matéria

---

### 4) Cadastro de Matéria
*Objetivo:* adicionar uma nova matéria no sistema  
*Campos:* nome, descrição (opcional)  
*Ações:* salvar, cancelar

---

### 5) Detalhe da Matéria
*Objetivo:* visualizar informações completas de uma matéria  
*Exibe:*
- nome
- descrição
- progresso atual (percentual)
- status
- observações (se existirem)
*Ações:*
- atualizar progresso

---

### 6) Atualizar Progresso
*Objetivo:* registrar avanço do usuário em uma matéria  
*Campos:*
- percentual (0–100)
- status (ex: não iniciado / em andamento / concluído)
- observação (opcional)
*Ações:* salvar, cancelar

---

## Regras de Navegação (Usabilidade)

- O usuário deve sempre ter um caminho claro para voltar ao Dashboard ou Matérias
- A ação “Cadastrar Matéria” deve ser visível na Home e na Lista de Matérias
- Atualizar Progresso deve estar disponível dentro do Detalhe da Matéria
- Feedback visual (mensagens de sucesso/erro) em todas as operações

---

## Conclusão

A arquitetura foi desenhada para reduzir fricção e facilitar o controle do estudo,
garantindo que o usuário visualize rapidamente seu progresso e consiga atualizar dados sem esforço.