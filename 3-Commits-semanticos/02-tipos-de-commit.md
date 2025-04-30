# 02 - Tipos de Commit

## 🦄 Commits Semânticos e suas Intenções

Cada tipo de commit representa uma **intenção clara**. Esses tipos são essenciais para a compreensão do que está sendo alterado no projeto e ajudam a manter o histórico limpo e organizado.

Abaixo, listamos os principais tipos usados no padrão [Conventional Commits](https://www.conventionalcommits.org/pt-br/v1.0.0/), com explicações e exemplos práticos.

---

## 🗂️ Tabela de Tipos de Commit

| Tipo        | Descrição                                                                                       | Relacionado ao SemVer |
|-------------|--------------------------------------------------------------------------------------------------|------------------------|
| `feat`      | Adiciona uma nova funcionalidade ao projeto                                                      | **MINOR**             |
| `fix`       | Corrige um bug ou erro                                                                            | **PATCH**             |
| `docs`      | Alterações na documentação (ex: README, comentários, etc.)                                        | —                      |
| `test`      | Adição ou modificação de testes (unitários, integração, etc.)                                      | —                      |
| `build`     | Alterações que afetam o sistema de build ou dependências externas                                 | —                      |
| `perf`      | Melhorias de desempenho (sem alteração de comportamento)                                           | **PATCH**             |
| `style`     | Mudanças que não afetam a lógica: espaçamentos, ponto e vírgula, formatação, etc.                | —                      |
| `refactor`  | Refatorações que não alteram funcionalidades (ex: melhorar legibilidade, reaproveitar código)     | —                      |
| `chore`     | Tarefas administrativas (ex: atualização de configs, ajustes de linter, .gitignore, etc.)         | —                      |
| `ci`        | Alterações relacionadas à integração contínua (CI)                                                 | —                      |
| `revert`    | Reversão de um commit anterior                                                                    | —                      |
| `raw`       | Mudanças em arquivos de configuração, dados brutos ou parâmetros                                   | —                      |
| `cleanup`   | Remoção de código morto, comentários desnecessários, arquivos temporários                         | —                      |
| `remove`    | Exclusão de arquivos, diretórios ou funcionalidades obsoletas ou não utilizadas                   | —                      |

---

## ✍️ Exemplos de Commits na Prática

```bash
feat(login): criar formulário de login
fix(auth): corrigir erro na validação de senha
docs(readme): adicionar instruções de instalação
style(home): padronizar indentação e espaços
refactor(api): extrair lógica de autenticação
perf(image): otimizar carregamento de imagens
chore(gitignore): incluir arquivos de ambiente
revert: revert "feat(ui): adicionar dark mode"
```

> 💡 Dica: mantenha o **verbo no infinitivo impessoal** (ex: “adicionar” e não “adicionado” ou “adicionando”).

---

## 📌 Boas práticas

- Escreva mensagens **curtas, objetivas e significativas**.
- Use **um commit para cada alteração lógica**.
- Combine tipos com escopos quando fizer sentido: `feat(api)`, `fix(login)`, etc.
- Não use commits genéricos como `update`, `ajustes`, `mudanças`.

---

## 🎯 Conclusão

Saber **qual tipo de commit utilizar** ajuda a manter seu repositório limpo, compreensível e pronto para escalar. No próximo arquivo, você verá **exemplos reais** de como aplicar esses tipos em projetos do dia a dia.
