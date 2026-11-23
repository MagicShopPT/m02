Trabalho realizado por: *Vitor Silva* **13422**. Licenciatura em Informática, 2026.

# Módulo 02 — CSS3, Flexbox e Grid (Progresso até EX07)

Este ficheiro documenta a evolução progressiva da resolução dos exercícios práticos do **Módulo 02** da unidade curricular de Programação WEB (ISMT), atualizado até ao **EX07**.

## Lista de Exercícios Realizados

* [x] **EX01 — Selectors**: Aplicação de diferentes tipos de seletores CSS sem alterar a estrutura HTML fornecida.
* [x] **EX02 — Box Model**: Construção de uma coleção de cartões aplicando o modelo de caixa e comparação visual entre `content-box` e `border-box`.
* [x] **EX03 — Typography**: Estilização de uma página de documentação técnica com controlo tipográfico, esquema de cores e variáveis CSS.
* [x] **EX04 — Components**: Criação de uma biblioteca de componentes visuais reutilizáveis (badges, buttons, alerts, cards e forms) em CSS puro.
* [x] **EX05 — Flexbox Playground**: Construção de 6 layouts distintos explorando propriedades Flexbox e barra de navegação no topo.
* [x] **EX06 — Navigation Bar**: Criação de uma barra de navegação responsiva com logo, links, botão CTA, alinhamento Flexbox e menu mobile colapsável.
* [x] **EX07 — Photo Gallery**: Criação de uma galeria de fotografias responsiva com CSS Grid, múltiplas colunas, `gap`, itens de diferentes tamanhos e composição por `grid-template-areas`.

## Descrição dos Exercícios e Tomadas de Decisão

### EX01 — Selectors (Nível L1)
* **Objetivo:** Compreender e aplicar diferentes tipos de seletores CSS sobre uma estrutura HTML fixa.
* **Decisões tomadas:**
  * Respeitada integralmente a restrição de não alterar a estrutura do ficheiro `exemplo_exer1_CSS.html`, ligando apenas a folha de estilos externa `styles.css` no `<head>`.
  * Aplicados seletores de elemento (`body`, `header`, `section`, `h2`, `ul`, `li`, `label`, `button`), classe (`.destaque`), ID (`#nome`, `#email`), descendentes (`nav a`, `section p`), atributo (`input[type="text"]`, `input[type="email"]`, `button[type="submit"]`) e pseudo-classes (`:hover`, `:focus`, `:first-child`).
  * Implementados estados visuais de `:hover` e `:focus` (bónus) para garantir feedback imediato na navegação por rato e teclado.

### EX02 — Box Model (Nível L1)
* **Objetivo:** Compreender o funcionamento do Box Model (`width`, `padding`, `border`, `margin` e `box-sizing`) e prever com rigor as dimensões reais ocupadas pelos elementos.
* **Decisões tomadas:**
  * Construída uma coleção de cartões (`Cartão Base`, `Cartão Destaque` e `Cartão Compacto`) utilizando explicitamente `width`, `padding`, `border`, `margin` e `box-sizing: border-box` para manter a largura total previsível (`280px`) mesmo quando o espaçamento interno e a espessura da borda variam.
  * Implementada a secção bónus de comparação visual lado a lado entre `content-box` (onde `width: 280px` soma `40px` de padding horizontal e `10px` de border horizontal, perfazendo `330px` reais) e `border-box` (onde os `280px` já englobam padding e border).

### EX03 — Typography (Nível L2)
* **Objetivo:** Controlar a tipografia, a hierarquia de leitura e o esquema de cores de uma página de documentação técnica.
* **Decisões tomadas:**
  * Implementado um sistema centralizado de variáveis CSS (`Custom Properties`) em `:root` (bónus) e aplicado via `var(--nome)` para gerir paleta cromática, famílias tipográficas (`--font-sans` e `--font-mono`), escala de tamanhos, alturas de linha (`--leading-body: 1.65` e `--leading-heading: 1.25`) e pesos tipográficos.
  * Definidos estilos específicos para títulos (`h1`, `h2`, `h3`), blocos de código (`code` e `pre`) e ligações (`a`, `a:hover`, `a:focus`), assegurando contraste elevado e boa legibilidade.

### EX04 — Components (Nível L2)
* **Objetivo:** Criar componentes visuais reutilizáveis com CSS3 puro e estilos consistentes.
* **Decisões tomadas:**
  * Desenvolvidos os cinco grupos de componentes exigidos (**Badges**, **Buttons**, **Alerts**, **Cards** e **Forms**) sem recorrer a Bootstrap ou Tailwind.
  * Centralizada a identidade visual através de variáveis CSS (`:root`) para cores semânticas, raios de borda e anel de foco (`--focus-ring`), garantindo coerência visual e acessibilidade por teclado.

### EX05 — Flexbox Playground (Nível L1)
* **Objetivo:** Compreender o alinhamento e a distribuição unidimensional de elementos com CSS Flexbox.
* **Decisões tomadas:**
  * Criados 6 cenários de demonstração (superando o mínimo de 5 exigido) para isolar e testar `flex-direction`, `justify-content`, `align-items`, `flex-wrap`, `gap`, `flex-grow` e `flex-shrink`.
  * Incluída uma barra de navegação fixa no topo construída com Flexbox (bónus), alinhando marca, ligações e botão de ação.

### EX06 — Navigation Bar (Nível L2)
* **Objetivo:** Construir uma barra de navegação responsiva alinhada com Flexbox e adaptável a diferentes larguras de ecrã.
* **Decisões tomadas:**
  * Estruturada a barra com logótipo, lista de ligações e botão de ação (*CTA*) distribuídos através de `display: flex`, `justify-content: space-between` e `align-items: center`.
  * Implementado o bónus de menu mobile colapsável abaixo de `768px` utilizando apenas CSS (`#menu-toggle:checked` com ícone hambúrguer animado), eliminando a dependência de JavaScript e evitando *scroll* horizontal.

### EX07 — Photo Gallery (Nível L2)
* **Objetivo:** Utilizar o sistema bidimensional CSS Grid para organizar uma galeria de fotografias responsiva com itens de diferentes dimensões.
* **Decisões tomadas:**
  * Construída a galeria principal com `display: grid`, `grid-template-columns: repeat(3, 1fr)`, `gap: 18px` e cartões em destaque a ocupar duas colunas (`grid-column: span 2`), assegurando imagens responsivas através de `width: 100%` e `object-fit: cover`.
  * Implementada a secção bónus recorrendo a `grid-template-areas` e `grid-area` (`hero`, `side-top`, `side-bottom`, `strip-1`, `strip-2`, `strip-3`), com reorganização fluida por media queries para tablet (`<= 820px`) e smartphone (`<= 540px`).

## Tecnologias Utilizadas

* HTML5 semântico
* CSS3 (Seletores, Box Model, Tipografia, Variáveis CSS, Componentes, Flexbox, CSS Grid e Media Queries)

## Como Executar

1. Abrir a pasta do módulo (`m02`) no Visual Studio Code.
2. Navegar até à diretoria do exercício pretendido (`ex01/` a `ex07/`) e abrir o ficheiro `.html` correspondente num navegador web ou através da extensão **Live Server**.

## Estrutura do Projeto (até EX07)

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
|   ├── index.html
|   ├── styles.css
|   └── README.md
└── README.md
```

#### Autor

**Vitor Silva** (N.º **13422**)

* GitHub: [MagicShopPT](https://github.com/MagicShopPT)