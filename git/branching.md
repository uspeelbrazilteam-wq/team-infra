# Git, Branches

## Estrutura

| Branch | Descrição |
|--------|-----------|
| `main` | Código estável e revisado. **Protegida.** |
| `feature/*` | Desenvolvimento de funcionalidades ou conteúdo. |
| `fix/*` | Correções de bugs. |
| `docs/*` | Alterações exclusivamente em documentação. |

---

## Proteção de `main`

A branch `main` está configurada com proteção no GitHub:

- Push direto **bloqueado** para todos os membros.
- Merge permitido somente via Pull Request com ao menos **1 aprovação**.
- Branch deve estar atualizada com `main` antes do merge.

**Qualquer tentativa de push direto para `main` será rejeitada NA HORA.**

---

## Nomenclatura de Branches

Use o prefixo correspondente ao tipo de trabalho, seguido de um identificador curto e descritivo em kebab-case.

```
feature/modelagem-expressao-proteica
feature/pagina-team-wiki
fix/erro-calculo-rendimento
docs/atualiza-protocolo-transformacao
```

---

## Criação e Exclusão

```bash
# Criar branch a partir de main atualizada
git checkout main && git pull origin main
git checkout -b feature/nome

# Excluir branch local após merge
git branch -d feature/nome

# Excluir branch remota após merge
git push origin --delete feature/nome
```

Branches mergeadas devem ser excluídas do remoto para manter o repositório organizado.

## Regra

Branches devem existir apenas durante desenvolvimento ativo.
Branches antigas devem ser removidas imediatamente após merge.

