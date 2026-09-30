# BEVEX24 Design System

## Princípio universal

Os produtos compartilham a mesma qualidade de experiência, não a mesma aparência. Arquitetura de componentes, tipografia, espaçamento, acessibilidade, estados e comportamento são universais; a paleta e os elementos de personalidade pertencem a cada produto e devem representar sua área de atuação.

Um produto novo no formato `...Flow` precisa definir sua identidade setorial antes da implementação. Não deve herdar automaticamente a cor principal da BEVEX24, do LabFlow ou do FactoryFlow.

## Identidade institucional BEVEX24

| Papel | Token | Valor |
| --- | --- | --- |
| Marca principal | `--bevex-cyan` | `#06B6D4` |
| Marca profunda | `--bevex-cyan-deep` | `#0E7490` |
| Navegação e texto forte | `--bevex-ink` | `#102A33` |
| Canvas | `--bevex-canvas` | `#F8FAFC` |
| Texto secundário | `--bevex-slate` | `#64748B` |
| Sucesso | `--bevex-success` | `#16A34A` |
| Atenção | `--bevex-warning` | `#D97706` |
| Falha | `--bevex-danger` | `#DC2626` |

Esses tokens identificam o site institucional, o portal oficial e os sistemas administrativos próprios da BEVEX24. Eles não são o tema padrão obrigatório dos produtos `...Flow`.

## Famílias de produtos

| Produto | Área | Identidade principal | Cores de apoio | Sensação desejada |
| --- | --- | --- | --- | --- |
| **BEVEX24** | Institucional e sistemas oficiais | Ciano | Azul-petróleo, grafite e branco | Tecnologia, conexão e confiança |
| **LabFlow** | Gestão laboratorial ambiental e clínica | Verde-água / teal | Azul clínico, verde ambiental e branco | Precisão, ciência e cuidado |
| **FactoryFlow** | Gestão operacional industrial | Âmbar | Carvão quente, cobre e areia | Operação, energia e chão de fábrica |
| **...Flow** | Nova área de atuação | Cor definida pelo domínio | Neutros e complementares próprios | Reconhecimento imediato do setor |

Cada produto deve fornecer a mesma escala semântica de tokens (`brand-50` a `brand-800`, `canvas`, `surface`, `ink`, `muted`, `line` e `sidebar`). O valor desses tokens muda por produto; os componentes consomem tokens e não cores institucionais fixas.

Títulos usam **Manrope** e controles/textos usam **Inter**, com fallback para fontes do sistema. Espaçamento parte de 4 px; raios principais usam 8, 12 e 16 px.

## Navegação comercial

A sidebar deve oferecer marca + produto, workspace atual, módulos agrupados, estado do sistema e perfil do usuário. Em desktop pode recolher para um rail de 80–88 px; em mobile usa drawer com backdrop. A página ativa precisa de texto, contraste e indicador visual — nunca apenas cor.

- Departamentos expansíveis usam chevron vetorial arredondado, sem depender de glifos da fonte do sistema.
- A abertura usa movimento curto e suave, respeitando `prefers-reduced-motion`.
- As opções abertas ficam dentro de um painel de contraste leve em relação à sidebar.
- Não usar linha vertical para representar a hierarquia do submenu.
- Apenas um departamento fica aberto por vez e o estado é exposto com `aria-expanded` e `aria-hidden`.

## Componentes e estados

- Botão primário usa a cor acessível do produto; ações destrutivas continuam vermelhas e cores semânticas não mudam de significado.
- Inputs com label persistente, erro junto ao campo e foco visível.
- Tabelas com cabeçalho claro, densidade consistente e estado vazio distinto de erro.
- Carregamento, vazio, parcial, indisponível e sucesso são estados diferentes.
- Movimento respeita `prefers-reduced-motion`.
- Contraste mínimo WCAG AA e alvos de toque de pelo menos 40 px quando possível.
