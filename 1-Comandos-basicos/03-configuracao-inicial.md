# 03 - Configuração Inicial do Git

Após instalar o Git, é essencial fazer uma configuração inicial. Isso garante que todas as alterações feitas no repositório fiquem associadas corretamente ao seu nome e e-mail. Essa configuração só precisa ser feita uma vez por máquina.

---

## 👤 Configurar nome e e-mail

Abra o terminal e execute os seguintes comandos:

```bash
git config --global user.name "Seu Nome"
git config --global user.email "seu@email.com"
```

Substitua pelos seus dados reais. Exemplo:

```bash
git config --global user.name "Cristiano Benites"
git config --global user.email "cristiano@example.com"
```

> Esses dados aparecerão em cada commit que você fizer.

---

## 🔍 Verificar as configurações

Para conferir se os dados foram salvos corretamente:

```bash
git config --list
```

Você deve ver uma saída parecida com:
```
user.name=Cristiano Benites
user.email=cristiano@example.com
```

---

## ⚙️ Outras configurações úteis

### Definir editor padrão (opcional):

```bash
git config --global core.editor "code --wait"
```

Esse comando define o VS Code como editor padrão. Se estiver usando outro, substitua `code` por `nano`, `vim`, `notepad`, etc.

### Exibir cores nos comandos:
```bash
git config --global color.ui auto
```

---

## 🗂️ Onde essas configurações ficam salvas?

As configurações globais do Git ficam salvas em um arquivo chamado `.gitconfig`, localizado na sua pasta de usuário:

- **Linux/macOS**: `~/.gitconfig`
- **Windows**: `C:\Users\seu-usuario\.gitconfig`

Você pode abrir esse arquivo com qualquer editor de texto para ver ou editar as configurações manualmente.

---

## 🎯 Conclusão

Agora você está com o Git configurado com a sua identidade. Isso é essencial para colaborar em projetos e garantir a autoria correta dos seus commits.

> No próximo arquivo, você aprenderá os principais comandos Git para iniciar seus projetos e controlar versões com eficiência.
