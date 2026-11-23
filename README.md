Trabalho realizado por: *Vitor Silva* **13422**. Licenciatura em Informática, 2026.

# Módulo 02 — CSS3, Flexbox e Grid

Este repositório contém a resolução completa dos exercícios práticos do **Módulo 02** da unidade curricular de Programação WEB do Instituto Superior Miguel Torga (ISMT — 2026/2027).

## Lista de Exercícios Realizados
- [x] **EX01 — Selectors** *(Nível L1)*: Aplicação de seletores CSS (elemento, classe, ID, descendentes, atributos e pseudo-classes) sem alterar o HTML fornecido.
- [x] **EX02 — Box Model** *(Nível L1)*: Coleção de cartões aplicando `width`, `padding`, `border`, `margin` e `box-sizing`, com comparação visual entre `content-box` e `border-box`.
- [x] **EX03 — Typography** *(Nível L2)*: Estilização de documentação técnica com controlo tipográfico, esquema de cores e sistema de variáveis CSS.
- [x] **EX04 — Components** *(Nível L2)*: Criação de componentes visuais reutilizáveis (cards, buttons, alerts, badges e forms) em CSS puro.
- [x] **EX05 — Flexbox Playground** *(Nível L1)*: Construção de 6 layouts variados explorando propriedades Flexbox e barra de navegação.
- [x] **EX06 — Navigation Bar** *(Nível L2)*: Barra de navegação responsiva com logo, links, botão CTA e menu mobile em CSS puro.
- [x] **EX07 — Photo Gallery** *(Nível L2)*: Galeria de fotografias responsiva utilizando CSS Grid, múltiplos tamanhos e `grid-template-areas`.
- [x] **EX08 — Dashboard** *(Nível L3)*: Estrutura de dashboard com Header, Sidebar, Main, Cards, Table e Footer em CSS Grid e versão mobile.
- [x] **EX09 — Responsive Challenge** *(Nível L4)*: Landing page *Mobile First* adaptável a 320px, 768px, 1024px e 1440px, sem *scroll* horizontal e com modo escuro.

## Descrição dos Exercícios e Tomadas de Decisão

### EX01 — Selectors (Nível L1)
* **Objetivo:** Compreender e aplicar diferentes tipos de seletores CSS sobre uma estrutura HTML fixa.
* **Decisões tomadas:**
  * Respeitada a restrição de não alterar o código HTML de `exemplo_exer1_CSS.html`, ligando apenas a folha de estilos externa `styles.css`.
  * Aplicados seletores de elemento, classe (`.destaque`), ID (`#nome`, `#email`), descendentes (`nav a`, `section p`), atributo (`input[type="text"]`, `input[type="email"]`, `button[type="submit"]`) e pseudo-classes (`:hover`, `:focus`, `:first-child`).
  * Incluídos estados visuais de `:hover` e `:focus` (bónus) para melhorar a interação e acessibilidade por teclado.

### EX02 — Box Model (Nível L1)
* **Objetivo:** Compreender o cálculo de dimensões no Box Model e a diferença entre `content-box` e `border-box`.
* **Decisões tomadas:**
  * Criada uma coleção de cartões (`Cartão Base`, `Cartão Destaque` e `Cartão Compacto`) com `width: 280px`, `padding`, `border`, `margin` e `box-sizing: border-box` para garantir dimensões externas consistentes independentemente da espessura da borda ou preenchimento interno.
  * Desenvolvida uma comparação visual (bónus) entre `content-box` (`330px` de largura real ocupada) e `border-box` (`280px` de largura total) para demonstrar na prática o impacto no layout.

### EX03 — Typography (Nível L2)
* **Objetivo:** Controlar tipografia, escala hierárquica e cores numa página de documentação técnica.
* **Decisões tomadas:**
  * Criado um sistema de variáveis CSS (`Custom Properties`) em `:root` (bónus) para centralizar cores, fontes (`--font-sans` e `--font-mono`), tamanhos, pesos e alturas de linha (`line-height`), facilitando a manutenção e consistência visual.
  * Estilizados títulos (`h1` a `h3`), blocos de código técnico (`code`, `pre`) e estados de ligações (`a`, `:hover`, `:focus`) com contraste adequado.

### EX04 — Components (Nível L2)
* **Objetivo:** Criar componentes visuais reutilizáveis com CSS puro e estilos consistentes.
* **Decisões tomadas:**
  * Construídos os cinco componentes solicitados (**Badges**, **Buttons**, **Alerts**, **Cards** e **Forms**) sem recorrer a Bootstrap ou Tailwind.
  * Uniformizada a linguagem visual com variáveis CSS (`:root`) para variantes semânticas, espaçamentos, estados `:hover` / `:disabled` e foco visível para acessibilidade.

### EX05 — Flexbox Playground (Nível L1)
* **Objetivo:** Compreender o funcionamento do Flexbox através da construção de múltiplos layouts.
* **Decisões tomadas:**
  * Desenvolvidos 6 layouts distintos (superando o mínimo de 5 layouts) para demonstrar `flex-direction`, `justify-content`, `align-items`, `flex-wrap`, `gap`, `flex-grow` e `flex-shrink`.
  * Implementada uma barra de navegação Flexbox no topo como bónus.

### EX06 — Navigation Bar (Nível L2)
* **Objetivo:** Criar uma barra de navegação responsiva com alinhamento Flexbox.
* **Decisões tomadas:**
  * Alinhados logótipo, ligações e botão CTA com Flexbox (`justify-content: space-between` e `align-items: center`).
  * Adicionado o bónus de menu mobile colapsável abaixo de `768px` com CSS puro (`#menu-toggle:checked`), assegurando navegação funcional em dispositivos móveis e desktop.

### EX07 — Photo Gallery (Nível L2)
* **Objetivo:** Utilizar CSS Grid para construir uma galeria de fotografias responsiva com múltiplos tamanhos.
* **Decisões tomadas:**
  * Implementada uma grelha de múltiplas colunas com `gap`, imagens responsivas (`width: 100%` e `object-fit: cover`) e cartões alargados (`grid-column: span 2`).
  * Adicionada a composição bónus baseada em `grid-template-areas` e `grid-area`, adaptada a tablet e smartphone através de media queries.

### EX08 — Dashboard (Nível L3)
* **Objetivo:** Construir um dashboard com Header, Sidebar, Main, Cards, Table e Footer utilizando CSS Grid para a estrutura principal.
* **Decisões tomadas:**
  * Estruturado o layout global em CSS Grid com `grid-template-areas` (`header`, `sidebar`, `main`, `footer`), integrando cartões de métricas em grelha adaptativa e tabela responsiva.
  * Implementado o bónus de versão mobile (`<= 768px`) colapsando a estrutura para uma única coluna vertical sem *overflow* horizontal.

### EX09 — Responsive Challenge (Nível L4)
* **Objetivo:** Construir uma *landing page* *Mobile First* funcional em 320px, 768px, 1024px e 1440px, sem frameworks e sem *scroll* horizontal.
* **Decisões tomadas:**
  * Estruturada com estilos base para ecrãs móveis (`320px+`) e evolução progressiva via *media queries* `min-width` (`768px`, `1024px` e `1440px`), mantendo `overflow-x: hidden` e contentores fluidos.
  * Adicionado o bónus de modo escuro automático (`prefers-color-scheme: dark`) e manual em CSS puro (`#theme-toggle:checked`) através de variáveis CSS.

## Estrutura do Repositório
```text
m02/
├── ex01/
│   ├── exemplo_exer1_CSS.html
│   ├── styles.css
│   └── README.md
├── ex02/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex03/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex04/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex05/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex06/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex07/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex08/
│   ├── index.html
│   ├── styles.css
│   └── README.md
├── ex09/
│   ├── index.html
│   ├── styles.css
│   └── README.md
└── README.md
```

## Tecnologias Utilizadas
- HTML5 semântico
- CSS3 (Seletores, Box Model, Tipografia, Variáveis CSS, Componentes, Flexbox, CSS Grid e Responsive Design Mobile First)

## Como Executar
1. Clonar ou abrir a pasta `m02` no Visual Studio Code.
2. Abrir o ficheiro `.html` da diretoria do exercício pretendido (`ex01/` a `ex09/`) no navegador web ou através da extensão **Live Server**.

#### Autor
**Vitor Silva** (N.º **13422**)
* GitHub: [MagicShopPT](https://github.com/MagicShopPT)