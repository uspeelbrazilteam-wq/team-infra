# Governança — Regras do Time

## Regras Obrigatórias

As regras abaixo aplicam-se a **todos os membros/lideres** em **todos os repositórios**, sem exceção.

---

### 1. Todo merge via Pull Request

Nenhuma alteração vai para `main` sem passar por um PR aprovado.

- PRs requerem ao menos **1 aprovação** de outro membro do time.
- PRs sem revisor designado não serão mergeados.
- A aprovação é de responsabilidade do revisor — revise com atenção.

**Violação:** push direto para `main` é bloqueado por configuração do repositório e será revertido se contornado.

---

### 2. Commits diretos em `main` são proibidos

`main` é branch protegida. Push direto está desabilitado no GitHub.

Qualquer trabalho deve ser feito em branch separada seguindo o padrão `feature/*`, `fix/*` ou `docs/*`.

---

### 3. Commits com mensagens claras

Todo commit deve ter mensagem no formato `<tipo>: <descrição>` conforme definido em `git/commits.md`.

Mensagens genéricas ou sem contexto (`update`, `fix`, `changes`) são consideradas violação desta regra e podem bloquear a aprovação do PR.

---

## Consequências

O descumprimento das regras acima implica:

1. Rejeição do PR pelo revisor.
2. Solicitação de reescrita do histórico (rebase/squash) antes de novo review.
3. Em casos recorrentes, remoção temporária de permissão de escrita no repositório.

---

## Exceções

Não há exceções para as regras 1 e 2. Para a regra 3, commits de merge automático gerados pelo GitHub estão isentos.

Dúvidas sobre aplicação das regras devem ser endereçadas à liderança técnica do time.

## Autoridade

A decisão final sobre aprovação de PRs e aplicação das regras é da liderança de SIS/HARD do time.

