
# Git — Padrão de Commits

## Formato

```
<tipo>: <descrição curta no imperativo>
```

A descrição deve ser objetiva, em letras minúsculas, sem ponto final.

---

## Tipos

| Tipo | Quando usar |
|------|-------------|
| `feat` | Nova funcionalidade ou conteúdo |
| `fix` | Correção de bug ou erro |
| `docs` | Alteração em documentação |
| `refactor` | Refatoração sem mudança de comportamento |
| `style` | Ajustes de formatação, CSS, layout |
| `chore` | Tarefas de manutenção, configs, dependências |

---

## Exemplos

```bash
feat: adiciona seção de resultados na wiki
fix: corrige link quebrado na página de sponsors
docs: atualiza protocolo de miniprep
refactor: reorganiza estrutura de componentes React
style: ajusta tipografia do header
chore: atualiza dependências do projeto
```

---

## Regras

- Um commit por alteração lógica — não agrupe mudanças não relacionadas.
- Mensagens em **português ou inglês**, mas consistente dentro do repositório.
- Evite mensagens genéricas: `fix stuff`, `update`, `changes` são inaceitáveis.
- Commits com múltiplas alterações distintas devem ser separados com `git add -p`.

## Regra

Commits são parte do histórico permanente. Não escreva mensagens que você não gostaria de ler em uma revisão externa.
