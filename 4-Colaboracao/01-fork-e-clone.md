# 01 - Fork e Clone

Ao trabalhar com repositórios no GitHub, especialmente projetos colaborativos ou open source, é comum utilizar dois processos iniciais:

- **Fork** → criar uma cópia do repositório no seu próprio GitHub.
- **Clone** → copiar esse repositório do GitHub para a sua máquina local.

---

## 🍴 O que é Fork?

O **fork** cria uma cópia completa de um repositório na sua conta do GitHub. Ele permite que você faça alterações livremente sem afetar o repositório original.

### Quando usar?
- Ao contribuir com repositórios de terceiros
- Ao adaptar um projeto existente para um novo uso

### Como fazer um Fork:
1. Acesse o repositório no GitHub
2. Clique no botão `Fork` no canto superior direito
3. Escolha sua conta

Pronto! Agora você tem sua própria cópia do repositório.

---

## 💻 O que é Clone?

O **clone** baixa o repositório da sua conta GitHub para o seu computador.

### Comando:
```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
```

> Substitua pelo link do seu repositório. Ele pode ser copiado ao clicar no botão verde `Code > HTTPS` no GitHub.

### Exemplo:
```bash
git clone https://github.com/cristianobenites/Curso_Github.git
```

Isso criará uma pasta chamada `Curso_Github` com todos os arquivos.

---

## 🛠️ O que fazer depois do clone?

1. Acesse a pasta do projeto:
```bash
cd Curso_Github
```

2. Comece a fazer alterações localmente
3. Depois, envie suas mudanças de volta para o seu GitHub usando `git add`, `git commit` e `git push`

---

## 🧠 Fork x Clone: Qual a diferença?

| Ação   | Onde ocorre       | Objetivo                                 |
|--------|-------------------|------------------------------------------|
| Fork   | No GitHub         | Copiar o repositório para sua conta      |
| Clone  | No seu computador | Trabalhar no código de forma local       |

---

## 🎯 Conclusão

- O **fork** é usado para criar sua cópia pessoal no GitHub.
- O **clone** é usado para trabalhar com essa cópia no seu computador.

> No próximo arquivo, vamos aprender a contribuir com projetos via **Pull Requests** (PR), que é a principal forma de colaboração em projetos GitHub.
