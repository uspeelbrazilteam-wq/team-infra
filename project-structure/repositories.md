# Estrutura do Projeto — Repositórios

## Repositórios Ativos

O time mantém quatro repositórios no GitHub da organização. Cada um tem escopo definido e não deve receber conteúdo fora do seu domínio.

---

### `wiki-site`

Repositório do site oficial submetido ao iGEM.

**Conteúdo:** código-fonte do site (HTML/CSS/JS ou framework utilizado), assets visuais, textos das páginas da wiki.

**Owners:** SIS/HARD.

---

### `drylab`

Repositório de modelagem.

**Conteúdo:** scripts de análise, modelos, notebooks, dados processados, documentação metodológica das abordagens computacionais.

**Owners:**    Lideranca de modelagem.

---

### `wetlab`

Repositório de protocolos e registros experimentais.

**Conteúdo:** protocolos laboratoriais (Markdown), registros de experimentos, resultados brutos, planilhas de dados experimentais.

**Owners:** lideranca de modelagem.

---

### `docs`

Repositório de documentação interna do time.

**Conteúdo:** guias de onboarding, governança, decisões técnicas (ADRs), atas de reunião, materiais de treinamento.

**Owners:** SIS./HARD.

---

## Regras Gerais

- Arquivos grandes (>50 MB) não devem ser commitados, usa o Git LFS ou armazenamento externo (Drive, etc.).
- Credenciais, tokens ou dados sensíveis **nunca** devem ser commitados em nenhum repositório.
- Cada repositório segue as mesmas regras de branching e PR definidas em `git/`.

## Isolamento

Não misture responsabilidades entre repositórios.

Se houver dúvida sobre onde algo pertence, está no lugar errado.
