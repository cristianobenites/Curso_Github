# 01 - Introdução aos Commits Semânticos

## 🧠 O que é um Commit?

Um **commit** é um registro de alteração no seu projeto. Ele funciona como uma “foto” do estado atual dos arquivos, com uma mensagem que explica o que foi feito.

### Exemplo simples:
```bash
git commit -m "atualizando arquivos"
```
Essa mensagem é válida, mas **muito vaga**. Commits assim dificultam o entendimento do histórico do projeto.

---

## 🤔 Por que melhorar as mensagens de commit?

Boas mensagens de commit:
- Ajudam você e outras pessoas a entenderem o histórico do projeto
- Facilitam a revisão de código
- Auxiliam na geração de changelogs automáticos
- Melhoram a organização em equipes e projetos open source

---

## ✅ O que são Commits Semânticos?

Os **Commits Semânticos (Semantic Commits)** seguem um padrão de escrita onde cada commit tem um significado claro, baseado na intenção da alteração feita.

### Estrutura geral:
```bash
<tipo>(escopo opcional): <mensagem clara e curta>
```

### Exemplo:
```bash
feat(auth): adicionar autenticação por token JWT
```

Esse padrão é conhecido como [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/) e é adotado por muitas empresas e projetos profissionais.

---

## 🚀 Vantagens dos Commits Semânticos

| Vantagem                          | Descrição                                                                 |
|----------------------------------|---------------------------------------------------------------------------|
| Clareza                          | Cada commit expressa claramente sua intenção                             |
| Automatização                    | Possibilita geração automática de changelogs                             |
| Versionamento Semântico         | Facilita a definição de `major`, `minor` e `patch`                       |
| Padronização                     | Cria uma cultura de código mais organizada e legível                     |

---

## 📌 Quando usar esse padrão?

Sempre que possível, mesmo em projetos pequenos. Além de ajudar na organização individual, o hábito prepara você para ambientes profissionais.

---

## 🎯 Conclusão

Commits semânticos ajudam a contar a história do projeto de forma lógica e rastreável. No próximo arquivo, você verá quais são os **tipos de commit** e quando utilizar cada um.

> Dica: você pode usar ferramentas como o **Commitizen** ou **GitMoji** para auxiliar na padronização.
