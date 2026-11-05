# Registro de Uso de IA — Entrega 1

**Projeto:** Scalla Seller — site institucional de agência de marketplaces
**Aluno:** Gabriel Silva Machado — RA 98039075
**Entrega:** 1 — Esqueleto Semântico (`entrega-1`)
**Ferramentas utilizadas:** Claude (Anthropic), para gerar e corrigir o site e para a primeira versão deste registro; ChatGPT (OpenAI), apenas para melhorar a redação e a organização deste registro (prompts 12 e 13)
**Data:** 05/11/2026

> Documento exigido pela seção 5 do enunciado do Projeto Integrador.

---

## 1. Mapeamento de Uso

### Código e arquivos

| Arquivo | Participação da IA | Observação |
|---|---|---|
| `index.html` | **Integral** | Estrutura e redação geradas por IA a partir do briefing |
| `catalogo.html` | **Integral** | Idem |
| `sobre.html` | **Integral** | Idem |
| `contato.html` | **Integral** | Idem |
| `img/*.png` | **Integral** | Imagens provisórias geradas por script Python (Pillow) |
| `README.md` | **Integral** | Idem |
| Este arquivo (seções 1, 2 e 4) | **Integral** | Escritas pelo Claude; o ChatGPT foi usado depois só para sugerir melhorias de redação e organização |
| Identificação dos pontos de revisão | **Integral** | A IA apontou pontos discutíveis no próprio código e um roteiro de onde alterar (prompt 6) |
| **Alterações da revisão técnica** | **Nenhuma** | A meu cargo: feitas por mim, direto no código, em commits meus |
| **Este arquivo (seção 3)** | **Nenhuma** | A meu cargo: justificativas escritas por mim |

### Conteúdo do site

Aqui há duas origens diferentes, e a distinção importa:

**Dados fornecidos por mim (informação real da empresa):**
- Nome da agência, sócios e paleta azul e branco.
- Os dois serviços (estruturação e gestão mensal) e as 7 frentes do
  acompanhamento 360: onboarding, pesquisa de mercado, precificação, anúncios,
  criativos, Ads e gestão contínua.
- Canais: Mercado Livre e Shopee; TikTok Shop fora do escopo atual.
- Todos os preços das tabelas.
- Condições: sem limite de SKUs; verba de Ads paga pelo cliente.
- Público: CNPJ de qualquer nicho, já vendendo ou começando.
- WhatsApp de contato: (35) 99968-1545.

**Redigido pela IA, a ser confirmado por mim antes de o site ir ao ar de verdade:**
- Todo o texto corrido (a redação das frases, não os fatos acima).
- O detalhamento das listas "O que entra" de cada serviço, no catálogo.
- Localização em Borda da Mata e horário de segunda a sexta, das 8h às 18h.
- Relatório mensal de acompanhamento para o cliente.
- Itens de "O que não está incluso" além da verba de Ads (logística, estoque e
  atendimento ao comprador final).
- Os números do painel ilustrativo (R$ 184 mil, 2.431 pedidos, ACOS de 9,4%),
  que são **fictícios** e estão identificados assim na própria página.
- **E-mail provisório:** `contato@scallaseller.com.br` é um exemplo até a
  agência ter o endereço oficial.

---

## 2. O que a IA fez

> Os prompts que enviei estão na íntegra no **Apêndice A**, no fim do documento,
> exatamente como foram escritos. Aqui fica o resumo do que cada ferramenta fez.

| Etapa | O que a IA fez |
|---|---|
| Prompt 1 | O Claude leu o enunciado e gerou de uma vez as 4 páginas em HTML puro (`index`, `catalogo`, `sobre`, `contato`), as imagens provisórias e o README |
| Prompt 2 e 3 | Reorganizou o site para a sugestão 2 do enunciado (pequeno negócio local): Home, Catálogo, Sobre e Contato |
| Prompt 4 | Revisou a própria saída e corrigiu os erros listados na seção 2.1 |
| Prompt 5 | Colocou o meu WhatsApp real e avisou que a seção 3 é minha, sem redigi-la |
| Prompt 6 | Apontou 3 pontos do código para eu revisar e onde ficam |
| Prompts 7 e 8 | Não pôde criar o repositório na minha conta; eu criei o vazio e ela enviou as branches `entrega-1` e `main` |
| Prompts 9 a 11 | Explicou o código página por página, ajudou a ativar o GitHub Pages e conferiu este registro |
| Prompts 12 e 13 | O ChatGPT sugeriu melhorias de redação e organização deste registro. Não mexeu no código e não escreveu a seção 3 |
| Prompts seguintes | O Claude me guiou nas minhas 3 alterações e conferiu os commits e a validação depois que eu fiz |

---

## 2.1 Correções feitas pela própria IA (prompts 4 e 5)

> Feitas pela ferramenta na própria saída, depois dos meus pedidos de revisão.
> **Não fazem parte da minha revisão técnica** (seção 3).

| Erro na versão gerada | Correção |
|---|---|
| Formulário com `method="post"`: o GitHub Pages recusa POST (erro 405) | `method` no padrão (GET) até haver back-end |
| Comentário errado sobre `<h3>` dentro de `<summary>` | `<h3>` removido e comentário corrigido |
| WhatsApp de exemplo que podia ser de uma pessoa real | Trocado por número fictício; depois, o meu número real |
| Compromissos comerciais e funções do sócio inventados pela IA (prazo de resposta, diagnóstico grátis, atendimento aos sábados etc.) | Removidos ou trocados por texto neutro |
| Legenda do painel parecia resultado real de cliente | Marcado como ilustrativo, números fictícios |
| Método 360 com 6 frentes em vez de 7 | Frente "Ads" adicionada |
| Imagens sem acento ("Gestao", "Evolucao") | Imagens geradas de novo |
| Cada pergunta do FAQ num `<article>` sem heading (W3C: "Article lacks heading") | `<article>` único envolvendo o FAQ |
| Home e README com detalhes inventados ou desatualizados | Textos igualados à página Sobre |

**Autoria dos commits:** os quatro primeiros commits da branch foram feitos pela
ferramenta com o meu usuário do git, sem marcação de coautoria. Depois deles, os
commits da IA trazem `Co-Authored-By: Claude`. Os commits da seção 3 são só meus.

---

## 3. Revisão Técnica — alterações feitas por mim

> **ESTA SEÇÃO AINDA PRECISA SER PREENCHIDA POR MIM, GABRIEL.**
>
> Não foi gerada por IA, de propósito: o enunciado avalia justamente a minha
> capacidade de auditar o código. Preencher isto com texto gerado seria
> exatamente o que a seção 5 quer evitar. Vale 15% da nota e sustenta a defesa
> final.
>
> **O que fazer:** escolher no mínimo 3 dos pontos de `PONTOS-PARA-REVISAO.md`,
> **alterar o código de fato** e documentar cada alteração no formato abaixo.
> Depois, apagar este bloco de aviso.

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

Além da revisão manual, o código passou por verificação automatizada:

- **W3C Nu HTML Checker** (`vnu.jar`), rodado direto nas 4 páginas:
  *"Document checking completed. No errors found."* O único aviso é informativo,
  sobre o suporte do atributo `inputmode` em navegadores antigos.
- **Nova rodada depois das minhas 3 alterações** (05/11/2026): o `vnu.jar` voltou
  a dar *"No errors found"* nas 4 páginas, com o mesmo aviso informativo.
- **Script de verificação estrutural** — hierarquia de headings, âncoras
  quebradas, `alt` ausente, `label` órfão, `th` sem `scope`, `id` duplicado,
  `aria-current` incorreto e presença indevida de CSS/JS. Nenhuma falha.

---

## Apêndice A — Prompts na íntegra

> Reproduzidos **como foram enviados**, com os mesmos erros de digitação.

### Prompt 1 — briefing inicial (com o PDF do enunciado anexado)

```
[Projeto Integrador](https://www.ead.univas.edu.br/pluginfile.php/206109/mod_assign/intro/Projeto%20Integrador.pdf)
O que deve ter nesta entrega:
As 4 páginas em HTML puro, sem CSS:
Estrutura, semântica, hierarquia de headings, navegação interna funcional e checklist de acessibilidade aplicado.
Formato de Entrega
Enviar o link do repositório [GitHub](https://github.com/), a entrega deve corresponder a uma branch ou tag específica no repositório, para esta entrega use o nome da branch como entrega-1


LEIA O CONTEXTO E FACA
```

### Prompts de ajuste e revisão

**Prompt 2.** Não foi texto digitado: a ferramenta perguntou o tema e eu cliquei em
`Scalla Seller — agência de marketplaces`.

**Prompt 3.** `faça com que entre na sugestão do tema, dentro do que ele propôs`
Resultado: site reorganizado para a sugestão 2 do enunciado (pequeno negócio local).

**Prompt 4.** `QUERO QUE REVISE E PROCURE ERROS E Arrume, ja esta no github? me explica o que foi feito e como, quero saber explicar e como eu mostro? a onde eiu vejo?`
Resultado: a IA corrigiu erros na própria saída (seção 2.1).

**Prompt 5.** `WhatsApp coloca o meu 35 999681545` / `sobre minha parte que eu tinha que fazer esta tudo certo? esta em formato humanizado? esta tudo coerente?`
Resultado: número real aplicado. A IA não redigiu a seção 3, que é minha.

**Prompt 6.** `preciso que em pontos para revisao voce me liste os 3 mais faceis de fazer com explicacoes o codigo e um passo a passo de como fazer isso la, em que linha, qual parte etc`

**Envio por engano.** Mandei duas imagens sem relação e escrevi `MANDEI ERRADO DESCONSIDERE, esqueça elas`.

**Prompt 7.** `voce ja nao subiu no meu github? crie o repo como scallaseller-projetointegrador algo assim`
Resultado: a IA não cria repositórios na minha conta; criei o repositório vazio.

**Prompt 8.** `Criei` Resultado: a IA enviou as branches `entrega-1` e `main`.

**Prompt 9.** `pronto, agora o que eu faco, me explique o codigo, como foi feito e como estao as coisas que eram partes minha?`

**Prompt 10.** Apenas uma captura de tela (página 404 do GitHub Pages), sem texto.
Resultado: a IA confirmou que o Pages não estava ativo e passou como ativar.

**Prompt 11.** `preciso que recapitule comigo, estou perdido. O que eu vou ter que fazer, como eu envio pra ele? como ficou a documentacao? inventou um prompt que eu te mandei?`
Resultado: a IA conferiu os prompts deste registro contra as minhas mensagens.

### Prompts ao ChatGPT (melhoria deste registro)

**Prompt 12.** `melhore isso e faca um prompt paranque eu coloque em registro ia e deixe ainda o que ela fez anotado`
Depois dele enviei o conteúdo deste registro como material para revisão.

**Prompt 13.** `voce que vai fazer, to falando pra melhorar as coisas que eu escrevi etc`
Resultado: o ChatGPT sugeriu melhorias de redação e de organização. Ele não mexeu
no código do site e não escreveu a seção 3.

> **Pendente de completar:** os prompts em que pedi ao Claude orientação sobre as
> alterações da revisão técnica serão acrescentados aqui, com o texto exato,
> antes da entrega.
