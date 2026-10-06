# AGENTS — Regras obrigatórias para agentes

> Este arquivo vale para qualquer agente de IA ou automação
> (OpenCode, Codex, Copilot, Claude, etc.) que modifique este repositório.

## 1. Regra de commit + push (OBRIGATÓRIA)

- **TODA alteração feita no código, arquivos ou documentação DEVE ser commitada e pushada.**
- Não deixe alterações apenas locais / não commitadas ao final da tarefa.
- Fluxo obrigatório ao concluir qualquer tarefa:
  1. `git status` — conferir o que mudou
  2. `git add -A` (ou `git add <arquivos específicos>`)
  3. `git commit -m "<tipo>: <descrição curta>"` (ex: `feat: ...`, `fix: ...`, `docs: ...`, `chore: ...`)
  4. `git push origin main` (ou para a branch atual, depois abrir PR se for o caso)
- Se o push falhar (ex: remote desatualizado), faça `git pull --rebase origin main` e tente o push novamente. Não finalize a tarefa com push pendente.
- Nunca use `git push --force` sem autorização explícita do usuário.

## 2. Convenções

- Branch principal: `main`
- Commits em português ou inglês, curtos e descritivos.
- Não commitar segredos (tokens, senhas, `.env`). Usar `.gitignore`.
