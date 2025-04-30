# 03 - Merge e Rebase

Ao trabalhar com branches no Git, você precisará eventualmente **juntar** o conteúdo de uma branch com outra. Para isso, usamos dois comandos principais:

- `git merge`
- `git rebase`

Ambos têm o mesmo objetivo: **integrar o trabalho de uma branch em outra**, mas o fazem de maneiras diferentes.

---

## 🔀 `git merge`

O `merge` cria um novo commit que une o histórico das duas branches.

### Exemplo:
```bash
git checkout main

git merge nova-feature
```

Esse comando irá juntar as alterações da `nova-feature` na `main`, criando um commit especial chamado “merge commit”.

### Vantagens:
- Mantém o histórico completo de tudo o que aconteceu.
- Mostra quando as branches se uniram.

### Desvantagens:
- Pode gerar um histórico mais poluído visualmente, com muitos nós e commits de merge.

---

## ♻️ `git rebase`

O `rebase` reescreve o histórico da sua branch, colocando seus commits como se fossem os últimos da branch de destino.

### Exemplo:
```bash
git checkout nova-feature

git rebase main
```

Isso move os commits da `nova-feature` para o topo da `main`, como se tivessem sido criados depois dela.

### Vantagens:
- Históricos mais lineares e limpos.
- Melhora a leitura de logs e revisões de código.

### Desvantagens:
- Reescreve o histórico (pode ser perigoso em branches compartilhadas).

⚠️ Nunca use `rebase` em branches que já foram enviadas para o GitHub e usadas por outras pessoas.

---

## 👥 Exemplo prático
Imagine que você está na branch `main`, e existe uma branch `login-form` com novos commits.

Para integrar:

**Usando merge:**
```bash
git checkout main
git merge login-form
```

**Usando rebase:**
```bash
git checkout login-form
git rebase main
```

> Ambas as formas funcionarão, mas o histórico final será diferente.

---

## 🔍 Comparativo Visual

| Ação     | Resultado                     |
|----------|-------------------------------|
| Merge    | Junta os históricos com commit de merge |
| Rebase   | Reescreve o histórico como se fosse contínuo |

---

## 🎯 Conclusão

- Use `merge` quando quiser preservar a história original das branches.
- Use `rebase` quando quiser um histórico mais limpo e linear.

> No próximo arquivo, veremos o que acontece quando há conflitos ao usar merge ou rebase e como resolvê-los corretamente.
