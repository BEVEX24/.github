# BEVEX Design System

## Identidade compartilhada

| Papel | Token | Valor |
| --- | --- | --- |
| Navegação e texto forte | `--bevex-navy` | `#0B1220` |
| Ação principal | `--bevex-blue` | `#2563EB` |
| Informação e conexão | `--bevex-cyan` | `#06B6D4` |
| Canvas | `--bevex-canvas` | `#F8FAFC` |
| Texto secundário | `--bevex-slate` | `#64748B` |
| Sucesso | `--bevex-success` | `#16A34A` |
| Atenção | `--bevex-warning` | `#D97706` |
| Falha | `--bevex-danger` | `#DC2626` |

Títulos usam **Manrope** e controles/textos usam **Inter**, com fallback para fontes do sistema. Espaçamento parte de 4 px; raios principais usam 8, 12 e 16 px.

## Produtos

- **FactoryFlow:** laranja `#EA580C` e âmbar `#F59E0B` como acentos industriais, sem substituir a base corporativa.
- **LabFlow:** ciano `#06B6D4` como acento laboratorial.

## Navegação comercial

A sidebar deve oferecer marca + produto, workspace atual, módulos agrupados, estado do sistema e perfil do usuário. Em desktop pode recolher para um rail de 80–88 px; em mobile usa drawer com backdrop. A página ativa precisa de texto, contraste e indicador visual — nunca apenas cor.

## Componentes e estados

- Botão primário azul; ações destrutivas vermelhas; acento do produto apenas para contexto.
- Inputs com label persistente, erro junto ao campo e foco visível.
- Tabelas com cabeçalho claro, densidade consistente e estado vazio distinto de erro.
- Carregamento, vazio, parcial, indisponível e sucesso são estados diferentes.
- Movimento respeita `prefers-reduced-motion`.
- Contraste mínimo WCAG AA e alvos de toque de pelo menos 40 px quando possível.
