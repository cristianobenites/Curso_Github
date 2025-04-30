# 01 - SemVer: Versionamento Semântico Básico

## 📦 O que é Versionamento Semântico?

O **Versionamento Semântico**, ou **SemVer**, é um padrão que define **como numerar versões de um software** para indicar claramente o tipo de mudanças feitas.

Ele usa o formato:

```bash
MAJOR.MINOR.PATCH
```

### Exemplo:
```bash
v2.4.1
```
Significa:
- **2** → Versão principal (MAJOR)
- **4** → Versão secundária (MINOR)
- **1** → Correção de bugs (PATCH)

---

## 🔢 Regras do SemVer

| Nível    | Quando aumentar        | Impacto esperado                       |
|----------|------------------------|----------------------------------------|
| MAJOR    | Quebra de compatibilidade | Usuários precisam adaptar seus projetos |
| MINOR    | Nova funcionalidade, mas compatível | Melhora sem quebrar o que já existe       |
| PATCH    | Correções de bugs      | Sem alterar comportamentos existentes  |

---

## 🧠 Por que usar SemVer?

- 🔍 Clareza: mostra rapidamente o tipo de atualização feita
- 🔧 Estabilidade: evita que atualizações quebrem projetos que dependem do seu
- 📊 Automação: permite que ferramentas atualizem dependências com segurança

---

## 🧪 Exemplos

### Atualização de segurança:
```bash
1.2.3 → 1.2.4
```
(só o PATCH muda)

### Nova funcionalidade compatível:
```bash
1.2.3 → 1.3.0
```
(só o MINOR muda)

### Grande mudança que quebra o sistema:
```bash
1.2.3 → 2.0.0
```
(MAJOR muda: pode quebrar compatibilidade)

---

## 🛠️ Boas práticas

- Mantenha um arquivo `CHANGELOG.md` explicando o que mudou em cada versão
- Combine SemVer com Commits Semânticos para versionamento automático (ex: `semantic-release`)
- Teste bem seu projeto antes de aumentar a versão MAJOR

---

## 🎯 Conclusão

Seguir o padrão SemVer ajuda a comunicar de forma clara e profissional as mudanças do seu projeto. No próximo arquivo, veremos **como aplicar o versionamento na prática** em repositórios Git e projetos hospedados no GitHub.
