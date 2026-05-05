# Git — Fluxo de Trabalho

## Fluxo Padrão

Todo trabalho no repositório segue este ciclo:

```
branch → commits → push → Pull Request → merge
```

---

## Etapas

### 1. Criar branch
Crie uma branch a partir de `main` atualizada.

```bash
git checkout main
git pull origin main
git checkout -b feature/nome-descritivo
```

### 2. Commitar alterações
Faça commits incrementais com mensagens claras.

```bash
git add .
git commit -m "feat: implementa parser de sequências FASTA"
```

### 3. Push para o remoto
Envie a branch para o repositório remoto.

```bash
git push origin feature/nome-descritivo
```

### 4. Abrir Pull Request
Abra um PR no GitHub apontando para `main`. Ver `pull-requests.md`.

### 5. Review e merge
Aguarde revisão de ao menos um membro do time. Após aprovação, o merge é realizado via interface do GitHub.

---

## Regras

- `main` nunca recebe push direto — apenas merges via PR aprovado.
- Branches desatualizadas devem ser sincronizadas com `main` antes do PR:

```bash
git fetch origin
git rebase origin/main
```

## Regra Crítica

Se não há Pull Request, a alteração não existe.

