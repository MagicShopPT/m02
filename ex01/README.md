Trabalho realizado por: *Vitor Silva* **13422**. Licenciatura em Informática, 2026.

# Módulo 02 — CSS3, Flexbox e Grid (Progresso até EX01)

Este documento apresenta a resolução progressiva dos exercícios práticos do **Módulo 02** da unidade curricular de Programação WEB (Instituto Superior Miguel Torga).

## Lista de Exercícios Realizados
- [x] **EX01 — Selectors**: Aplicação de diferentes tipos de seletores CSS sem alterar a estrutura HTML fornecida.

## Descrição dos Exercícios e Tomadas de Decisão

### EX01 — Selectors (Nível L1)
* **Objetivo:** Compreender e aplicar os principais tipos de seletores CSS (elementos, classes, IDs, descendentes, atributos e pseudo-classes) sobre uma página HTML já existente.
* **Decisões tomadas:**
  * **Integridade do HTML:** Manteve-se intacta toda a estrutura semântica do ficheiro `exemplo_exer1_CSS.html`, adicionando apenas a ligação externa `<link rel="stylesheet" href="styles.css">` no `<head>`.
  * **Seletores de Elemento, Classe e ID:** Foram definidos estilos base para elementos estruturais (`body`, `header`, `section`, `button`), realce visual através da classe `.destaque` e formatação específica para os identificadores únicos `#nome` e `#email`.
  * **Seletores Descendentes e de Atributo:** Utilizou-se `nav a` e `section p` para estilizar elementos dependentes do seu contexto, e seletores de atributo como `input[type="text"]`, `input[type="email"]` e `button[type="submit"]` para formatar os controlos do formulário sem necessidade de adicionar classes extra ao HTML.
  * **Bónus e Acessibilidade (`:hover` e `:focus`):** Implementaram-se estados `:hover` para resposta visual ao rato e `:focus` visível nos links, campos de texto e botão de submissão para garantir acessibilidade na navegação por teclado, além da pseudo-classe estrutural `li:first-child`.

## Tecnologias Utilizadas
- HTML5 (estrutura base fornecida)
- CSS3 (folha de estilos externa)

## Como Executar
1. Abra a pasta `m02` no Visual Studio Code.
2. Navegue até à diretoria `ex01/` e abra o ficheiro `exemplo_exer1_CSS.html` num navegador web ou através da extensão **Live Server**.

## Estrutura do Projeto (até EX01)
```text
m02/
├── ex01/
|   ├── exemplo_exer1_CSS.html
|   ├── styles.css
|   └── README.md
└── README.md
```

#### Autor
**Vitor Silva** (N.º **13422**)
* GitHub: [MagicShopPT](https://github.com/MagicShopPT)