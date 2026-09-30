# Contribuindo com projetos BEVEX24

## Fluxo

1. Crie uma branch `feat/`, `fix/`, `docs/` ou `chore/`.
2. Use Conventional Commits.
3. Abra um pull request pequeno, com objetivo, validação, risco e reversão.
4. Aguarde CI e revisão de código antes do merge.

## Regras comuns

- Testes e análise de dependências devem passar.
- Mudanças de banco são incrementais, idempotentes quando possível e documentadas.
- Autorização e validação pertencem ao servidor; a interface não é fronteira de segurança.
- Integrações externas precisam de timeout, erro explícito, idempotência e trilha de auditoria.
- Segredos, dados pessoais e bases reais não entram no Git.
- Interfaces seguem `docs/DESIGN_SYSTEM.md`, navegação por teclado, foco visível e contraste WCAG AA.
- Falhas de leitura não podem ser apresentadas como ausência de registros.
