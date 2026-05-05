
# Git — Pull Requests

## O que é um PR

Um Pull Request (PR) é a solicitação formal de merge de uma branch para `main`. É o único mecanismo permitido para integrar código ao repositório principal.

PRs garantem revisão antes do merge, registram o contexto da mudança e mantêm o histórico auditável.

---

## Como Abrir

1. Faça push da sua branch para o remoto.
2. No GitHub, entra no repositório e clique em **"Compare & pull request"**.
3. Defina:
   - **Base:** `main`
   - **Compare:** sua branch
   - **Título:** descritivo (mesmo padrão dos commits)
   - **Descrição:** o que foi feito e por quê
4. Adicione ao menos **1 revisor** do time.
5. Submeta o PR.

---

## Boas Práticas

**Escopo:** Um PR deve cobrir uma unidade de trabalho coesa. PRs com mudanças em múltiplas áreas não relacionadas dificultam a revisão e serão solicitados para divisão.

**Tamanho:** PRs menores são revisados mais rápido. Prefira PRs focados a grandes dumps de código.

**Descrição:** Inclua contexto suficiente para o revisor entender o que foi feito sem precisar executar o código.

**Draft PR:** Use PRs em rascunho (`Draft`) para trabalho em andamento que ainda não está pronto para revisão.

**Conflitos:** Resolva conflitos com `main` antes de solicitar revisão. PRs com conflitos não são mergeados.

---

## Processo de Review

- O revisor aprova ou solicita alterações via GitHub.
- O autor responde aos comentários e atualiza a branch conforme necessário.
- Após aprovação, o merge é realizado pelo autor ou pelo revisor designado.
- A branch é excluída após o merge.

## Responsabilidade

O autor é responsável pela qualidade do código.
O revisor é responsável por impedir a entrada de código mediocre em `main`.
