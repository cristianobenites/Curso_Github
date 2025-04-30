# 02 - Pull Request (PR)

Depois de fazer um fork e modificar um projeto no seu próprio repositório, você pode sugerir que as mudanças sejam incluídas no projeto original. Isso é feito através de um **Pull Request**.

## 🔄 O que é um Pull Request?

Um **Pull Request (PR)** é uma solicitação para que as suas alterações feitas em um repositório **forkado** sejam analisadas e, se aprovadas, **integradas ao repositório original**.

---

## 📋 Quando usar um PR?
- Quando você quer contribuir com um projeto que não é seu
- Quando trabalha em equipe e precisa que alguém revise seu código
- Quando deseja registrar uma funcionalidade implementada para ser discutida

---

## 🧭 Passo a passo para criar um Pull Request

### 1. Faça um Fork do repositório (já visto no módulo anterior)

### 2. Clone para sua máquina:
```bash
git clone https://github.com/seu-usuario/repositorio.git
```

### 3. Crie uma nova branch:
```bash
git checkout -b nome-da-sua-feature
```

### 4. Faça alterações no código e registre com commits:
```bash
git add .
git commit -m "feat: adicionar nova funcionalidade X"
```

### 5. Envie para o seu repositório remoto:
```bash
git push origin nome-da-sua-feature
```

### 6. Vá até o GitHub e clique no botão **Compare & pull request**

### 7. Escreva um título e uma descrição clara

Explique o que você fez e por que sua mudança é útil.

---

## 👀 O que acontece depois de um PR ser enviado?
- A equipe do repositório original **analisa** seu código
- Pode **pedir mudanças** (revisão de código)
- Pode **aprovar e fazer merge** da sua contribuição

---

## ✅ Boas práticas para Pull Requests

- Crie uma branch com nome significativo (`feature/menu-mobile`, `fix/navbar-responsiva`)
- Faça commits limpos e objetivos
- Escreva uma descrição clara e educada
- Teste suas alterações antes de enviar

---

## 🧠 Exemplo de fluxo

```bash
# 1. Criar branch
$ git checkout -b fix/ajuste-footer

# 2. Fazer alterações e commit
$ git add .
$ git commit -m "fix: corrigir espaçamento do footer"

# 3. Enviar para seu GitHub
$ git push origin fix/ajuste-footer
```

No GitHub, aparecerá um botão para criar o Pull Request a partir dessa branch.

---

## 🎯 Conclusão

Pull Requests são a principal forma de colaboração em projetos GitHub. Eles permitem que outras pessoas contribuam com segurança, mantendo o controle e a qualidade do código.

> No próximo arquivo, vamos entender como revisar o código de outras pessoas com responsabilidade e clareza.
