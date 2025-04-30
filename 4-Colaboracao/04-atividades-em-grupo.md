# 04 - Atividades em Grupo com Git e GitHub

Colaborar em equipe com Git e GitHub é uma habilidade essencial no mercado de tecnologia. Aqui, vamos apresentar **como estruturar atividades em grupo**, simular projetos reais e praticar a colaboração usando branches, commits, pull requests e revisão de código.

---

## 🧩 Estrutura Sugerida para Trabalhos em Equipe

### Cada grupo deve:
- Escolher um líder de repositório (responsável por criar e organizar o projeto)
- Criar um repositório no GitHub (público ou privado)
- Convidar os membros como colaboradores (via Settings > Collaborators)

---

## 🔀 Divisão por Branches

Cada pessoa pode trabalhar em uma **branch separada**:

```bash
git checkout -b nome-do-integrante/nome-da-feature
```

Exemplo:
```bash
git checkout -b joao/header
```

Essa estratégia evita conflitos e permite que todos colaborem ao mesmo tempo.

---

## 🛠️ Etapas sugeridas da atividade

1. **Planejamento do projeto** (definir funcionalidades e divisão)
2. **Criação da estrutura básica** do repositório
3. Cada membro:
   - Cria sua branch
   - Trabalha localmente
   - Faz commits claros e semânticos
   - Envia com `git push`
   - Abre um **Pull Request** com explicação do que fez
4. Outros colegas ou o líder fazem a **revisão (Code Review)**
5. Após aprovação, o PR é aceito e integrado à `main`

---

## 📦 Regras para a entrega

- Usar nomes de branch com padrão: `nome/funcionalidade`
- Usar commits semânticos com mensagens objetivas
- Nenhum código deve ir para a `main` sem passar por PR e revisão
- Ter pelo menos 1 commit por integrante
- O README.md deve conter:
  - Objetivo do projeto
  - Lista de integrantes
  - Instruções de execução

---

## ✅ Sugestão de Rubrica de Avaliação

| Critério                      | Pontos |
|------------------------------|--------|
| Uso correto do Git e GitHub  | 2,0    |
| Padrão de commits            | 2,0    |
| Organização por branches     | 2,0    |
| Clareza na colaboração (PRs) | 2,0    |
| Qualidade do código final    | 2,0    |

---

## 🎯 Conclusão

Trabalhar com Git e GitHub em grupo não é apenas sobre código, mas sobre **colaboração, organização e comunicação**. Pratique com seus colegas como se estivesse num time profissional.

> No próximo módulo, vamos falar sobre **versionamento semântico** e como numerar corretamente as versões de um projeto.
