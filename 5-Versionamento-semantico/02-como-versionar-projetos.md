# 02 - Como Versionar Projetos com Git e SemVer

Agora que você entendeu o que é o SemVer (Versionamento Semântico), vamos aprender **como aplicar esse padrão em projetos reais**, usando o Git e organizando as versões de forma clara e rastreável.

---

## 🔖 Onde declarar a versão do seu projeto?

- Em um arquivo `package.json` (em projetos Node.js)
- No `pyproject.toml` ou `setup.py` (em projetos Python)
- Em um campo `version:` (em arquivos de configuração)
- No `README.md` ou em um `VERSION.txt`

> O ideal é que a versão esteja **visível e padronizada** para quem utiliza ou colabora no projeto.

---

## 🛠️ Passo a passo: versionar manualmente

### 1. Atualize a versão do seu projeto
Por exemplo, se está mudando de `1.2.0` para `1.3.0`, edite isso em seu arquivo de versão:

```json
"version": "1.3.0"
```

### 2. Crie um commit com essa alteração:
```bash
git add .
git commit -m "chore(release): atualizar para v1.3.0"
```

### 3. Crie uma tag para marcar essa versão:
```bash
git tag v1.3.0
```

### 4. Envie a tag para o GitHub:
```bash
git push origin v1.3.0
```

Agora essa versão ficará registrada no GitHub como um “marco” no projeto.

---

## 🚀 Versionamento com GitHub Releases

1. No GitHub, vá até a aba **Releases** do repositório
2. Clique em **Draft a new release**
3. Preencha os campos:
   - **Tag version**: ex. `v1.3.0`
   - **Release title**: nome ou título da versão
   - **Descrição**: principais mudanças (pode usar o `CHANGELOG.md` como base)
4. Clique em **Publish release**

Isso facilita que outras pessoas saibam:
- O que foi alterado
- Qual versão estável devem usar
- Como fazer downgrade, se necessário

---

## ⚙️ Automatizando com Commits Semânticos + Semantic Release

Ferramentas como [`semantic-release`](https://github.com/semantic-release/semantic-release) geram automaticamente:
- Changelog
- Tags de versão
- Publicações de releases no GitHub/NPM

> Baseado nos tipos de commit (`feat`, `fix`, `BREAKING CHANGE`), ele calcula automaticamente se deve subir o PATCH, MINOR ou MAJOR.

---

## 🎯 Conclusão

- O versionamento claro ajuda seu projeto a crescer com estabilidade.
- Combine Git + SemVer + boas práticas de commits para gerar confiança no seu código.
- Aprender a criar releases bem documentadas é um diferencial profissional.

> No próximo módulo, você encontrará conteúdos extras para revisão, glossário e dicas de ferramentas que podem te ajudar no dia a dia com Git e GitHub.
