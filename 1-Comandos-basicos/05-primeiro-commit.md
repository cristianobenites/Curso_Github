# 05 - Primeiro Commit na Prática

Agora que você já conhece os comandos básicos do Git, vamos fazer juntos o seu **primeiro commit completo** em um projeto local. Essa é a etapa em que registramos oficialmente as alterações feitas em arquivos.

---

## 📁 1. Criar um novo projeto

Escolha um local no seu computador e crie uma nova pasta:

```bash
mkdir meu-primeiro-projeto-git
cd meu-primeiro-projeto-git
```

Dentro dessa pasta, crie um arquivo qualquer:
```bash
echo "# Meu Primeiro Projeto Git" > README.md
```

---

## 🔃 2. Iniciar o Git no projeto

```bash
git init
```
Esse comando transforma a pasta em um repositório Git.

---

## 📋 3. Verificar o status

```bash
git status
```
Você verá que o arquivo `README.md` está como "untracked" (não versionado ainda).

---

## ➕ 4. Adicionar arquivos para controle de versão

```bash
git add README.md
```
Ou para adicionar tudo:
```bash
git add .
```

---

## ✅ 5. Realizar o commit

```bash
git commit -m "feat: adicionar README inicial"
```
Isso registra sua alteração com uma mensagem curta e objetiva.

> ✅ Parabéns! Você acabou de fazer seu primeiro commit com Git.

---

## 📝 Dica: use mensagens claras nos commits

Uma boa mensagem ajuda você e os outros colaboradores a entenderem o histórico do projeto.

Use o formato:
```bash
<tipo>: <mensagem breve>
```
Exemplo:
```bash
feat: criar página inicial do site
```

> Veremos mais sobre commits semânticos no módulo 3.

---

## 🧪 Verificar o histórico de commits

```bash
git log --oneline
```
Isso mostra os commits realizados de forma resumida.

---

## 📌 Conclusão

Você iniciou um repositório, adicionou um arquivo e fez seu primeiro commit. Esse é o ciclo mais básico de uso do Git e é a base para todas as outras operações futuras.

> No próximo módulo, você aprenderá sobre como trabalhar com **branches** e criar fluxos de trabalho mais avançados.
