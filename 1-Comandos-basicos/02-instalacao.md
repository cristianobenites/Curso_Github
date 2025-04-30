# 02 - Instalação do Git

Antes de começar a usar o Git, precisamos instalá-lo no seu sistema. A instalação é simples e varia de acordo com o sistema operacional que você está usando.

---

## 💻 Instalação no Windows

1. Acesse o site oficial do Git: [https://git-scm.com](https://git-scm.com)
2. Clique em **Download for Windows**.
3. Execute o instalador `.exe` baixado.
4. Durante a instalação, mantenha as opções padrão (recomendado para iniciantes).
5. Finalize e abra o **Git Bash**, que será seu terminal para comandos Git.

> 🧠 O Git Bash é um terminal especial que permite usar comandos Unix no Windows.

---

## 🍎 Instalação no macOS

### Opção 1: Via Homebrew (recomendado)
```bash
brew install git
```

> Certifique-se de que o [Homebrew](https://brew.sh) esteja instalado.

### Opção 2: Via instalador
1. Acesse: [https://git-scm.com](https://git-scm.com)
2. Baixe a versão para macOS.
3. Siga as instruções da instalação.

---

## 🐧 Instalação no Linux

### Debian/Ubuntu:
```bash
sudo apt update
sudo apt install git
```

### Fedora:
```bash
sudo dnf install git
```

### Arch Linux:
```bash
sudo pacman -S git
```

---

## 🔍 Verificando a Instalação

Após instalar, digite no terminal:
```bash
git --version
```

Você deve ver algo como:
```
git version 2.42.0
```

Se esse comando funcionar, o Git está corretamente instalado!

---

## 🎯 Conclusão

Você agora tem o Git instalado e pronto para uso. No próximo módulo, aprenderemos como configurá-lo pela primeira vez e associar sua identidade aos commits.

> 📌 Dica: instale também o [GitHub CLI](https://cli.github.com/) se quiser interagir com o GitHub diretamente pelo terminal.
