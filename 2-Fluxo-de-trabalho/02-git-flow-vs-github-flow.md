# 02 - Git Flow vs GitHub Flow

Quando trabalhamos em equipe com Git, é importante seguir um **fluxo de trabalho (workflow)**. Isso organiza as branches e define como os desenvolvedores colaboram no projeto.

Neste arquivo, vamos comparar dois modelos muito usados:

- **Git Flow** → mais estruturado, ideal para grandes projetos.
- **GitHub Flow** → mais simples e ágil, ideal para times pequenos e projetos em andamento contínuo.

---

## 🧩 O que é Git Flow?

O **Git Flow** é um modelo clássico e bem estruturado de desenvolvimento com Git. Ele define várias branches com funções específicas:

### Principais branches:
- `main` (ou `master`) – versão final e estável em produção.
- `develop` – branch de desenvolvimento com o que está em andamento.

### Branches auxiliares:
- `feature/*` – para desenvolver novas funcionalidades.
- `release/*` – para preparar uma nova versão.
- `hotfix/*` – para corrigir erros críticos direto na produção.

### Ciclo resumido:
1. Criar branch `feature/nome` a partir de `develop`
2. Finalizar a feature e fazer merge na `develop`
3. Quando pronto para publicar, criar uma `release` e testar
4. Fazer merge da `release` na `main` e na `develop`
5. Se houver problema urgente, criar `hotfix` a partir da `main`

📌 **Vantagens**:
- Controle rígido de versões
- Ideal para grandes equipes e projetos complexos

⚠️ **Desvantagens**:
- Mais burocracia e branches para gerenciar
- Menos ágil para mudanças rápidas

---

## 🌐 O que é GitHub Flow?

O **GitHub Flow** é um fluxo mais moderno e simples, muito usado em projetos open source ou times ágeis.

### Como funciona:
1. Tudo começa a partir da branch `main`
2. Criar uma branch `feature-x` para cada funcionalidade
3. Trabalhar na feature e fazer commits
4. Abrir um **Pull Request** (PR) para a `main`
5. Outro membro revisa e aprova o PR
6. Fazer merge com `main` e deletar a branch

📌 **Vantagens**:
- Fluxo leve e direto
- Facilita o uso de CI/CD (integração e entrega contínua)
- Ideal para times pequenos e deploys frequentes

⚠️ **Desvantagens**:
- Pode ser arriscado se não houver revisão adequada
- Menos controle sobre versões em ambientes corporativos grandes

---

## 🔍 Comparativo

| Item                | Git Flow                        | GitHub Flow                       |
|---------------------|----------------------------------|-----------------------------------|
| Complexidade        | Alta                             | Baixa                             |
| Estrutura de branches | Várias (`develop`, `release`, etc.) | Apenas `main` e branches de features |
| Ideal para          | Projetos grandes com versões     | Projetos ágeis e open source      |
| Controle de versão  | Muito rigoroso                   | Mais flexível                     |

---

## 🎯 Qual usar?

Depende do contexto:
- Para **aulas, projetos pessoais ou times pequenos** → GitHub Flow
- Para **empresas com times grandes, versões fechadas e testes rigorosos** → Git Flow

> O mais importante é que **toda a equipe use o mesmo modelo**, para manter a organização.

---

No próximo arquivo, veremos como juntar branches usando os comandos `merge` e `rebase`, com exemplos práticos.
