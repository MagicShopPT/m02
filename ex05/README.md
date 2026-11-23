Trabalho realizado por: *Vitor Silva* **13422**. Licenciatura em Informática, 2026.

# Módulo 02 — CSS3, Flexbox e Grid (Progresso até EX05)

Este ficheiro documenta a evolução progressiva da resolução dos exercícios práticos do **Módulo 02** da unidade curricular de Programação WEB (ISMT), atualizado até ao **EX05**.

## Lista de Exercícios Realizados
- [x] **EX01 — Selectors**: Aplicação de diferentes tipos de seletores CSS sem alterar a estrutura HTML fornecida.
- [x] **EX02 — Box Model**: Construção de uma coleção de cartões aplicando o modelo de caixa e comparação visual entre `content-box` e `border-box`.
- [x] **EX03 — Typography**: Estilização de uma página de documentação técnica com controlo tipográfico, esquema de cores e variáveis CSS.
- [x] **EX04 — Components**: Criação de uma biblioteca de componentes visuais reutilizáveis (badges, buttons, alerts, cards e forms) em CSS puro.
- [x] **EX05 — Flexbox Playground**: Construção de 6 layouts distintos explorando propriedades Flexbox e barra de navegação no topo.

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

## Tecnologias Utilizadas
- HTML5 semântico
- CSS3 (Seletores, Box Model, Tipografia, Variáveis CSS, Componentes e Flexbox)

## Como Executar
1. Abrir a pasta do módulo (`m02`) no Visual Studio Code.
2. Navegar até à diretoria do exercício pretendido (`ex01/` a `ex05/`) e abrir o ficheiro `.html` correspondente num navegador web ou através da extensão **Live Server**.

## Estrutura do Projeto (até EX05)
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
|   ├── index.html
|   ├── styles.css
|   └── README.md
└── README.md
```

#### Autor
**Vitor Silva** (N.º **13422**)
* GitHub: [MagicShopPT](https://github.com/MagicShopPT)