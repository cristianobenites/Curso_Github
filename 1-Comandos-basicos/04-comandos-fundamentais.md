# 04 - Comandos Fundamentais do Git

Agora que você já instalou e configurou o Git, é hora de aprender os **comandos fundamentais** que serão usados no seu dia a dia ao versionar projetos.

---

## 🆕 Iniciar um novo repositório Git

```bash
git init
```
Esse comando cria uma nova pasta oculta chamada `.git` no seu projeto. É onde o Git armazena todo o histórico.

> Use dentro da pasta onde está seu projeto.

---

## 📥 Clonar um repositório remoto (ex: do GitHub)

```bash
git clone <url-do-repositorio>
```
Exemplo:
```bash
git clone https://github.com/usuario/nome-do-projeto.git
```
Esse comando cria uma cópia local do repositório remoto.

---

## 📌 Verificar o status do repositório

```bash
git status
```
Mostra quais arquivos foram modificados, adicionados ou estão prontos para commit.

---

## ➕ Adicionar arquivos para commit

```bash
git add nome-do-arquivo
```
Ou para adicionar todos os arquivos modificados:
```bash
git add .
```

> Essa etapa prepara os arquivos para serem registrados no histórico.

---

## ✅ Fazer um commit

```bash
git commit -m "mensagem descritiva"
```
Exemplo:
```bash
git commit -m "feat: criar componente de login"
```
> O commit registra as mudanças no repositório com uma mensagem.

---

## 🔄 Ver histórico de commits

```bash
git log
```
Mostra todos os commits com hash, autor, data e mensagem.

Dica: use `git log --oneline` para visualizar de forma resumida.

---

## 🔄 Atualizar repositório local com mudanças do GitHub

```bash
git pull
```
Traz todas as atualizações do repositório remoto para seu repositório local.

---

## ⬆️ Enviar alterações locais para o GitHub

```bash
git push
```
Envia os commits do seu computador para o repositório remoto no GitHub.

> É necessário já ter vinculado o repositório remoto com `git remote add origin ...` e ter feito o `push` inicial.

---

## 🔁 Resumo dos Comandos Fundamentais

| Comando         | Descrição                                  |
|----------------|----------------------------------------------|
| `git init`     | Inicia um novo repositório Git              |
| `git clone`    | Clona um repositório remoto                 |
| `git status`   | Mostra o status dos arquivos                |
| `git add`      | Adiciona arquivos para serem commitados     |
| `git commit`   | Registra mudanças com uma mensagem          |
| `git log`      | Exibe o histórico de commits                |
| `git pull`     | Baixa atualizações do repositório remoto    |
| `git push`     | Envia commits para o repositório remoto     |

---

## 🎯 Conclusão

Esses são os comandos mais usados no dia a dia com o Git. Com eles, você já consegue iniciar projetos, registrar suas alterações e sincronizar com o GitHub.

> No próximo arquivo, você aprenderá como fazer seu primeiro commit na prática, passo a passo!
