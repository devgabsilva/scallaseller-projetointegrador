# Registro de Uso de IA — Entrega 1

**Projeto:** Scalla Seller — site institucional de agência de marketplaces
**Aluno:** Gabriel Silva Machado — RA 98039075
**Entrega:** 1 — Esqueleto Semântico (`entrega-1`)
**Ferramenta utilizada:** Claude (Anthropic), modelo Opus 5
**Data:** 05/11/2026

> Documento exigido pela seção 5 do enunciado do Projeto Integrador.

---

## 1. Mapeamento de Uso

Declaração honesta do que foi gerado por IA e do que não foi.

| Arquivo | Participação da IA | Observação |
|---|---|---|
| `index.html` | **Integral** | Estrutura e redação gerados por IA a partir do briefing abaixo |
| `servicos.html` | **Integral** | Idem |
| `planos.html` | **Integral** | Idem |
| `contato.html` | **Integral** | Idem |
| `img/*.png` | **Integral** | Imagens placeholder geradas por script Python (Pillow) |
| `README.md` | **Integral** | Idem |
| Este arquivo (seções 1 e 2) | **Integral** | — |
| **Este arquivo (seção 3)** | **Nenhuma** | Revisão técnica feita pelo aluno |
| **Conteúdo de negócio** | **Nenhuma** | Preços, serviços, canais, escopo e condições comerciais são dados reais da empresa, fornecidos pelo aluno |

**Resumo:** o código HTML desta entrega foi gerado integralmente com apoio de IA
a partir de um briefing meu, e em seguida auditado e modificado por mim conforme
a seção 3. O conteúdo de negócio — valores, serviços e condições — é informação
real da minha própria empresa e não foi inventado pela ferramenta.

---

## 2. Prompts Utilizados (na íntegra)

### Prompt 1 — briefing inicial

> *(acompanhado do PDF do enunciado do Projeto Integrador)*

```
O que deve ter nesta entrega:
As 4 páginas em HTML puro, sem CSS:
Estrutura, semântica, hierarquia de headings, navegação interna funcional
e checklist de acessibilidade aplicado.

Formato de Entrega
Enviar o link do repositório GitHub, a entrega deve corresponder a uma
branch ou tag específica no repositório, para esta entrega use o nome da
branch como entrega-1

LEIA O CONTEXTO E FACA
```

### Prompt 2 — definição do tema

A ferramenta perguntou qual seria o tema antes de gerar qualquer código, já que
errar o tema implicaria refazer as quatro páginas. Minha resposta:

```
Scalla Seller — agência de marketplaces
```

### Contexto adicional fornecido

Além dos prompts acima, a ferramenta teve acesso a dados da empresa que eu havia
registrado anteriormente e que foram usados como conteúdo real do site:

- Serviços: estruturação de loja e gestão mensal, com acompanhamento 360
  (onboarding, pesquisa de mercado, precificação, anúncios, criativos, Ads,
  gestão contínua).
- Canais: Mercado Livre e Shopee; TikTok Shop fora do escopo atual.
- Preços: estruturação R$ 1.500 por marketplace ou R$ 2.100 no combo
  ML + Shopee; gestão mensal R$ 1.300 por conta (R$ 900/mês no anual) ou
  R$ 1.900 no combo (R$ 1.500/mês no anual).
- Condições: sem limite de SKUs; verba de Ads paga pelo cliente.
- Público: CNPJ de qualquer nicho, já vendendo ou começando.
- Identidade visual: paleta azul e branco.

**Nenhum outro prompt foi utilizado nesta entrega.**

---

## 3. Revisão Técnica — alterações feitas por mim

> **ESTA SEÇÃO AINDA PRECISA SER PREENCHIDA POR MIM, GABRIEL.**
>
> Ela não foi gerada por IA de propósito: o enunciado avalia justamente a minha
> capacidade de auditar o código, e preencher isto com texto gerado seria
> exatamente o que a seção 5 quer evitar. Vale 15% da nota e é o que sustenta
> a defesa final.
>
> **O que fazer:** escolher no mínimo 3 dos pontos listados em
> `PONTOS-PARA-REVISAO.md`, **alterar o código de fato**, e documentar cada
> alteração no formato abaixo. Depois, apagar este bloco de aviso.

### Alteração 1

**O que a IA gerou:**

```html

```

**O que foi alterado:**

```html

```

**Por que foi alterado:**



---

### Alteração 2

**O que a IA gerou:**

```html

```

**O que foi alterado:**

```html

```

**Por que foi alterado:**



---

### Alteração 3

**O que a IA gerou:**

```html

```

**O que foi alterado:**

```html

```

**Por que foi alterado:**



---

## 4. Validação independente

Além da revisão manual, o código foi submetido a verificação automatizada:

- **W3C Nu HTML Checker** (`html5validator`) — 4 páginas, **zero erros**.
- **Script próprio de verificação** — hierarquia de headings, âncoras quebradas,
  `alt` ausente, `label` órfão, `th` sem `scope`, `id` duplicado, `aria-current`
  incorreto e presença indevida de CSS/JS. Nenhuma falha.
