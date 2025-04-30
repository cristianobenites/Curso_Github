# 03 - Code Review (Revisão de Código)

## 🧠 O que é Code Review?

**Code Review** (revisão de código) é o processo em que um desenvolvedor analisa o código escrito por outra pessoa antes que ele seja integrado ao projeto.

O objetivo é **garantir a qualidade do código**, evitar bugs, compartilhar conhecimento e manter a padronização do projeto.

---

## 🤝 Por que fazer revisão de código?

| Benefício                  | Explicação                                                                 |
|---------------------------|-----------------------------------------------------------------------------|
| Qualidade do código       | Identifica problemas antes de chegar à produção.                          |
| Aprendizado em equipe     | Quem escreve e quem revisa aprendem com o processo.                       |
| Padronização              | Garante que todos sigam o mesmo estilo e estrutura.                      |
| Menos bugs                | Reduz erros simples que poderiam passar despercebidos.                    |

---

## 👀 Como revisar um Pull Request

### 1. Leia com atenção a **descrição do PR**
- O que foi feito?
- Por que foi feito?
- Há relação com alguma issue ou bug?

### 2. Revise o código com critérios técnicos
- Está seguindo os padrões do projeto?
- O código é legível, organizado e eficiente?
- Há código duplicado ou desnecessário?
- Foi adicionado teste para a nova funcionalidade?

### 3. Faça comentários construtivos
- Elogie o que foi bem feito
- Sinalize pontos que podem ser melhorados
- Seja sempre respeitoso e claro

Exemplo de comentário:
```markdown
Ótimo trabalho! Só sugiro extrair essa lógica para uma função separada para facilitar testes e reutilização. O que acha?
```

### 4. Teste o código localmente (se possível)
- Isso ajuda a garantir que o PR realmente funciona como descrito

### 5. Escolha uma ação:
- ✅ **Aprovar o PR**
- ❌ **Solicitar mudanças** com sugestões claras

---

## ✍️ Dicas de comunicação na revisão
- Seja direto, mas educado
- Explique o porquê das sugestões
- Evite julgamentos pessoais

> “Esse código pode causar erro em X situação. Podemos refatorar assim: …”

---

## 🧰 Ferramentas de Code Review no GitHub
- Comentários linha a linha no PR
- Aprovação ou solicitação de alterações
- Histórico de revisões

---

## 🎯 Conclusão

A revisão de código é uma etapa fundamental em projetos colaborativos. Ela fortalece a equipe, melhora o projeto e eleva a qualidade do código entregue.

> No próximo arquivo, vamos explorar como trabalhar em equipe com atividades práticas de colaboração usando branches e pull requests.
