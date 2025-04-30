# 01 - O que é Branch?

## 🌿 Conceito de Branch

Uma **branch (ramo)** é uma cópia independente da linha principal de desenvolvimento de um projeto. Ela permite que você desenvolva funcionalidades, corrija bugs ou experimente novas ideias **sem afetar diretamente o código principal (geralmente chamado de `main` ou `master`)**.

### Analogia simples:
Imagine que o projeto principal é o **tronco de uma árvore**. Cada **branch** é um galho onde você pode desenvolver algo novo. Depois, você pode unir (fazer *merge*) esse galho de volta ao tronco.

---

## 🎯 Para que serve uma Branch?

- Trabalhar em funcionalidades isoladas sem atrapalhar o restante do projeto.
- Evitar conflitos entre pessoas da equipe desenvolvendo ao mesmo tempo.
- Permitir testes, protótipos ou refatorações com segurança.

---

## 🔧 Comandos básicos com Branches

### Criar uma nova branch
```bash
git branch nome-da-branch
```

### Mudar para uma branch existente
```bash
git checkout nome-da-branch
```

### Criar e já trocar para a nova branch
```bash
git checkout -b nome-da-branch
```

### Ver todas as branches
```bash
git branch
```
A branch atual será destacada com um asterisco `*`.

---

## 👩‍💻 Exemplo prático

```bash
git checkout -b nova-funcionalidade
```
Você começa a desenvolver nesta nova branch. Quando terminar, pode voltar para a principal:
```bash
git checkout main
```

Depois, pode unir a branch nova com a principal (veremos isso nos próximos arquivos).

---

## ⚠️ Boas práticas com Branches

- Dê nomes significativos às branches: `login-feature`, `fix-header`, `ajuste-footer`
- Trabalhe sempre em branchs diferentes da principal
- Faça commits pequenos e descritivos em cada branch

---

## 📌 Conclusão

Branches são essenciais para um desenvolvimento seguro, organizado e colaborativo. Dominar seu uso é o primeiro passo para trabalhar bem em equipe e manter seu código sempre estável.

> No próximo arquivo, veremos como diferentes estratégias de fluxo de trabalho utilizam as branches de formas diferentes (Git Flow vs GitHub Flow).
