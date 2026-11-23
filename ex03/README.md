Trabalho realizado por: *Vitor Silva* **13422**. Licenciatura em Informática, 09/10/2026.

# Módulo 02 — CSS3, Flexbox e Grid (Progresso até EX03)

Este ficheiro documenta a evolução progressiva da resolução dos exercícios práticos do Módulo 02 da unidade curricular de Programação WEB (ISMT), atualizado até ao **EX03**.

## Lista de Exercícios Realizados
- [x] **EX01 — Selectors**: Estilização de uma página HTML existente através de diferentes seletores CSS sem alterar a marcação HTML.
- [x] **EX02 — Box Model**: Construção de uma coleção de cartões aplicando o modelo de caixa e comparação visual entre `content-box` e `border-box`.
- [x] **EX03 — Typography**: Estilização de uma página de documentação técnica com controlo de tipografia, cores e sistema de variáveis CSS.

## Descrição dos Exercícios e Tomadas de Decisão

### EX01 — Selectors
* **Objetivo:** Compreender e aplicar diferentes tipos de seletores CSS sobre uma estrutura HTML fixa.
* **Decisões tomadas:**
  * Respeitada integralmente a restrição de não alterar a estrutura do ficheiro `exemplo_exer1_CSS.html`, ligando apenas a folha de estilos externa `styles.css` no `<head>`.
  * Aplicados seletores de elemento (`body`, `header`, `section`, `h2`, `ul`, `li`, `label`, `button`), classe (`.destaque`), ID (`#nome`, `#email`), descendentes (`nav a`, `section p`), atributo (`input[type="text"]`, `input[type="email"]`, `button[type="submit"]`) e pseudo-classes (`:hover`, `:focus`, `:first-child`).
  * Implementados estados visuais de `:hover` e `:focus` (bónus) para garantir feedback imediato na navegação por rato e teclado.

### EX02 — Box Model
* **Objetivo:** Compreender o funcionamento do Box Model (`width`, `padding`, `border`, `margin` e `box-sizing`) e prever com rigor as dimensões reais ocupadas pelos elementos.
* **Decisões tomadas:**
  * Construída uma coleção de cartões (`Cartão Base`, `Cartão Destaque` e `Cartão Compacto`) utilizando explicitamente `width`, `padding`, `border`, `margin` e `box-sizing: border-box` para manter a largura total previsível (`280px`) mesmo quando o espaçamento interno e a espessura da borda variam.
  * Implementada a secção bónus de comparação visual lado a lado entre `content-box` (onde `width: 280px` soma `40px` de padding horizontal e `10px` de border horizontal, perfazendo `330px` reais) e `border-box` (onde os `280px` já englobam padding e border).

### EX03 — Typography
* **Objetivo:** Controlar a tipografia, a hierarquia de leitura e o esquema de cores de uma página de documentação técnica.
* **Decisões tomadas:**
  * Implementado um sistema centralizado de variáveis CSS (`Custom Properties`) em `:root` (bónus) e aplicado via `var(--nome)` para gerir paleta cromática, famílias tipográficas (`--font-sans` e `--font-mono`), escala de tamanhos, alturas de linha (`--leading-body: 1.65` e `--leading-heading: 1.25`) e pesos tipográficos.
  * Definidos estilos específicos para títulos (`h1`, `h2`, `h3`), blocos de código (`code` e `pre`) e ligações (`a`, `a:hover`, `a:focus`), assegurando contraste elevado e boa legibilidade.

## Tecnologias Utilizadas
- HTML5
- CSS3 (Seletores, Box Model, Tipografia e Custom Properties / Variáveis CSS)

## Como Executar
1. Abrir a pasta do módulo (`m02`) no Visual Studio Code.
2. Abrir o ficheiro HTML do exercício pretendido (`ex01/exemplo_exer1_CSS.html`, `ex02/index.html` ou `ex03/index.html`) num navegador web ou através da extensão **Live Server**.

## Estrutura do Projeto (até EX04)
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
└── README.md
```

#### Autor
**Vitor Silva** (Nº 13422)
* GitHub: [MagicShopPT](https://github.com/MagicShopPT)