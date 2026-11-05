# Scalla Seller — Projeto Integrador

**Disciplina:** Interface Web com HTML e CSS
**Aluno:** Gabriel Silva Machado — RA 98039075
**Instituição:** UNIVÁS — Sistemas de Informação
**Entrega atual:** Entrega 1 — Esqueleto Semântico (branch `entrega-1`)

---

## Tema

**Sugestão 2 do enunciado — Site de pequeno negócio local.**

O negócio é a **Scalla Seller**, agência de gestão de contas em marketplaces
(Mercado Livre e Shopee) sediada em Borda da Mata, no Sul de Minas. O site
existe para apresentar o negócio, expor o catálogo de serviços com os preços
praticados e capturar solicitações de diagnóstico.

### Como as páginas mapeiam a sugestão do professor

O enunciado propõe, para a sugestão 2: *Home, Cardápio/Catálogo, Sobre,
Localização/Horários e Contato com formulário de reserva ou pedido.*

| Página proposta no enunciado | Página deste projeto | Arquivo |
|---|---|---|
| Home | Home | `index.html` |
| Cardápio / Catálogo | Catálogo de serviços e preços | `catalogo.html` |
| Sobre | Sobre a agência | `sobre.html` |
| Localização / Horários | Seção "Localização e horários" | dentro de `contato.html` |
| Contato com formulário | Contato, com formulário de diagnóstico | `contato.html` |

Como o escopo mínimo exige **no mínimo 4 páginas** e a entrega pede 4,
"Localização/Horários" foi consolidada dentro de `contato.html` como seção
própria, com `id` e entrada no sumário da página — o conteúdo proposto está
todo presente, agrupado onde o usuário naturalmente o procura.

---

## Estrutura de arquivos

```
.
├── index.html       Home — o que fazemos, para quem é, o que o cliente acompanha
├── catalogo.html    Catálogo — os dois serviços, tabelas de preços e condições
├── sobre.html       Sobre — quem conduz as contas, método 360 e canais
├── contato.html     Contato — formulário, localização e horários, canais, FAQ
├── img/
│   ├── logo-scalla-seller.png   Logotipo (placeholder, alt descritivo)
│   ├── painel-vendas.png        Imagem de conteúdo (alt descritivo)
│   └── ornamento.png            Imagem decorativa (alt vazio)
├── REGISTRO-IA.md   Registro de Uso de IA exigido pela seção 5 do enunciado
└── README.md
```

As quatro páginas são **arquivos HTML independentes**, conectadas por uma
navegação que se repete no `<header>` e no `<footer>` de todas elas — não são
seções de uma página só.

---

## Como visualizar

- **Site no ar (GitHub Pages):** `https://devgabsilva.github.io/scalla-seller/`
- **Código desta entrega:** branch
  [`entrega-1`](https://github.com/devgabsilva/scalla-seller/tree/entrega-1)
- **No computador, sem internet:** baixar o repositório e abrir o
  `index.html` no navegador.
- **Validar no W3C:** colar o endereço do site em
  <https://validator.w3.org/nu/>.

---

## Escopo desta entrega

A Entrega 1 é **HTML puro, sem CSS**. Nenhuma página contém `<style>`,
atributo `style`, `<link rel="stylesheet">` ou `<script>`. As páginas são
propositalmente feias: o que está sendo avaliado é o documento, não a aparência.

A estilização (Flexbox/Grid, variáveis CSS, 3 breakpoints) entra na
Entrega 2, na branch `entrega-2`.

### Dados provisórios

O e-mail de contato e os números do painel da home são provisórios. Eles estão
identificados no próprio código e no [`REGISTRO-IA.md`](REGISTRO-IA.md) e serão
trocados pelos dados oficiais da agência antes da versão final. O WhatsApp já é
o número real.

---

## Checklist de acessibilidade aplicado

| Item | Como foi aplicado | Onde conferir |
|---|---|---|
| **`lang`** | `<html lang="pt-BR">` nas 4 páginas | linha 2 de cada arquivo |
| **Skip link** | Primeiro elemento focável do `<body>`, aponta para `#conteudo`; o `<main>` recebeu `tabindex="-1"` para que o foco do teclado realmente se mova | topo do `<body>` |
| **Landmarks** | `header`, `nav`, `main`, `section`, `article`, `aside` e `footer` em todas as páginas; um único `<main>` por página | estrutura geral |
| **Landmarks rotulados** | Cada `<nav>` tem `aria-label` próprio (há mais de uma navegação por página); cada `<aside>` usa `aria-labelledby` apontando para seu próprio título | `aria-label` / `aria-labelledby` |
| **Hierarquia de headings** | Um `<h1>` por página, sem saltos de nível | validado por script, ver abaixo |
| **`alt` correto** | Imagens de conteúdo com `alt` descritivo; imagem decorativa com `alt=""`; logo dentro de link descreve o destino, não a aparência | `img/` |
| **Texto de link descritivo** | Nenhum "clique aqui"; links que abrem nova aba avisam no próprio texto | todas as páginas |
| **Tabelas de dados** | `<caption>` + `<th scope="col">` e `<th scope="row">` | `catalogo.html` |
| **Formulário** | `<label for>` em todos os campos, `<fieldset>`/`<legend>` nos grupos, `title` explicando o `pattern`, atributos `autocomplete` | `contato.html` |
| **Acordeão acessível** | FAQ em `<details>`/`<summary>` nativos: o navegador cuida do foco, das teclas Enter e Espaço e do estado aberto/fechado, sem JavaScript | `contato.html` |
| **Página atual** | `aria-current="page"` no item de menu correspondente | `<nav>` de cada página |
| **Navegação por teclado** | Só são usados elementos nativamente focáveis (`a`, `button`, `input`, `select`, `textarea`, `summary`). Nenhuma `div` ou `span` clicável, nenhum `tabindex` positivo | todas as páginas |

### Navegação interna funcional

- **Entre páginas:** menu no `header` e no `footer` das 4 páginas.
- **Dentro da página:** cada página tem um `<nav aria-label="Sumário desta página">`
  com âncoras para as suas próprias seções.
- **Entre seções de páginas diferentes:** por exemplo,
  `index.html` → `catalogo.html#estruturacao` e
  `catalogo.html` → `contato.html#formulario`.

Todas as âncoras foram verificadas: nenhuma aponta para um `id` inexistente.

---

## Validação executada

1. **Validador W3C (Nu HTML Checker)** — as 4 páginas passam com
   **zero erros**.

   ```bash
   java -jar vnu.jar --format text index.html catalogo.html sobre.html contato.html
   # Document checking completed. No errors found.
   ```

   O único aviso emitido é informativo (suporte do atributo `inputmode` em
   navegadores antigos) e foi mantido de forma deliberada: `inputmode="numeric"`
   abre o teclado numérico no celular e degrada sem prejuízo onde não há suporte.

2. **Verificação estrutural própria** — script que confere hierarquia de
   headings, âncoras quebradas, `alt` ausente, `label` órfão, `th` sem `scope`,
   `id` duplicado, `aria-current` incorreto e presença de CSS/JS indevido.
   Nenhuma falha.

---

## Decisões técnicas documentadas no código

As decisões de semântica e acessibilidade que não são óbvias à leitura estão
comentadas no próprio HTML, numeradas de 1 a 5, para serem defendidas na
avaliação final:

1. Skip link + `tabindex="-1"` no `<main>` — `index.html`
2. `aria-label` nos `<nav>` quando há mais de uma navegação — `index.html`
3. `<ol>` em vez de `<ul>` quando a ordem é informação — `sobre.html`
4. `<table>` com `<caption>` e `scope` para dados tabulares — `catalogo.html`
5. `<label>` real em vez de `placeholder` como rótulo — `contato.html`

---

## Cronograma do projeto

| Branch | Entrega | Status |
|---|---|---|
| `entrega-1` | Esqueleto semântico em HTML puro | **atual** |
| `entrega-2` | CSS: Flexbox/Grid, variáveis, 3 breakpoints | pendente |
| `entrega-3` | Formulário validado, contraste e ajustes finais | pendente |

---

## Uso de IA

Conforme a seção 5 do enunciado, o registro completo está em
[`REGISTRO-IA.md`](REGISTRO-IA.md).
