# 04 - Conflitos de Merge (Merge Conflicts)

Quando dois ou mais desenvolvedores alteram **a mesma parte do mesmo arquivo** em branches diferentes, o Git não consegue decidir automaticamente qual versão manter. Isso gera um **conflito de merge**.

Conflitos são comuns, especialmente em equipes. Saber resolvê-los faz parte da rotina de qualquer pessoa desenvolvedora.

---

## 🔥 Quando acontece um conflito?

Exemplo:
1. Você e outra pessoa editaram a mesma linha do arquivo `index.html`, em branches diferentes.
2. Ao fazer `git merge` ou `git rebase`, o Git detecta o conflito.

---

## ⚠️ Como identificar um conflito?

Após o merge ou rebase, o Git mostrará uma mensagem como:
```bash
CONFLICT (content): Merge conflict in index.html
Automatic merge failed; fix conflicts and then commit the result.
```

E ao rodar:
```bash
git status
```
Você verá:
```
both modified:   index.html
```

---

## 🧾 O que o Git faz no arquivo?

O Git marca a área em conflito assim:

```html
<<<<<<< HEAD
<h1>Texto da sua branch</h1>
=======
<h1>Texto da outra branch</h1>
>>>>>>> nome-da-outra-branch
```

Você deve **editar manualmente o arquivo**, escolhendo o que deseja manter.

---

## ✅ Como resolver um conflito

1. Abra o arquivo com conflito
2. Escolha qual versão manter ou combine as duas
3. Apague os marcadores `<<<<<<<`, `=======` e `>>>>>>>`
4. Salve o arquivo
5. Marque o conflito como resolvido:
```bash
git add nome-do-arquivo
```
6. Finalize o merge:
```bash
git commit
```

> O commit é obrigatório mesmo que você já tenha feito antes.

---

## 🛠️ Dicas para lidar com conflitos

- Mantenha as branches atualizadas com `git pull`
- Faça commits pequenos e frequentes
- Combine trabalho em equipe com boa comunicação
- Use ferramentas gráficas para ajudar:
  - VS Code (detecta e destaca conflitos automaticamente)
  - GitKraken, GitHub Desktop, Sourcetree

---

## 🎯 Conclusão

Conflitos de merge são normais em projetos colaborativos. O importante é **entendê-los, manter a calma e resolver com clareza**.

> No próximo módulo, vamos estudar como escrever commits de forma profissional e padronizada usando a técnica de **commits semânticos**.
