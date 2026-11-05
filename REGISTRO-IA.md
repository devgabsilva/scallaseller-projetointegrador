# Registro de Uso de IA — Entrega 1

**Projeto:** Scalla Seller — site institucional de agência de marketplaces
**Aluno:** Gabriel Silva Machado — RA 98039075
**Entrega:** 1 — Esqueleto Semântico (`entrega-1`)
**Ferramenta utilizada:** Claude (Anthropic), modelos Opus 5 e Opus 5.5
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
| Este arquivo (seções 1, 2 e 4) | **Integral** | — |
| Identificação dos pontos de revisão | **Integral** | A IA apontou pontos discutíveis no próprio código e um roteiro de onde alterar (prompt 6) |
| **Alterações da revisão técnica** | **Nenhuma** | A meu cargo: feitas por mim no código, um commit para cada uma |
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

## 2. Prompts Utilizados (na íntegra)

> Os prompts estão reproduzidos **exatamente como foram enviados**, com as
> mesmas quebras de linha e os mesmos erros de digitação. As linhas
> "Resultado", fora dos blocos, descrevem o que aconteceu depois de cada prompt
> e não fazem parte deles.

### Prompt 1 — briefing inicial

*(com o PDF do enunciado anexado)*

```
[Projeto Integrador](https://www.ead.univas.edu.br/pluginfile.php/206109/mod_assign/intro/Projeto%20Integrador.pdf)
O que deve ter nesta entrega:
As 4 páginas em HTML puro, sem CSS:
Estrutura, semântica, hierarquia de headings, navegação interna funcional e checklist de acessibilidade aplicado.
Formato de Entrega
Enviar o link do repositório [GitHub](https://github.com/), a entrega deve corresponder a uma branch ou tag específica no repositório, para esta entrega use o nome da branch como entrega-1


LEIA O CONTEXTO E FACA
```

### Prompt 2 — definição do tema

**Não foi um texto digitado por mim.** Antes de gerar o código, a ferramenta
perguntou qual seria o tema e ofereceu três opções. Eu cliquei nesta:

```
Scalla Seller — agência de marketplaces
```

### Prompt 3 — alinhamento ao tema do enunciado

```
faça com que entre na sugestão do tema, dentro do que ele propôs
```

Resultado: a primeira versão tinha Home, Serviços, Planos e Contato, o que não
correspondia a nenhuma das cinco sugestões do professor. O site foi
reorganizado para a **sugestão 2 (site de pequeno negócio local)**, com Home,
Catálogo, Sobre e Contato, e Localização/Horários entrou como seção da página
de contato.

### Prompt 4 — revisão de erros

```
QUERO QUE REVISE E PROCURE ERROS E Arrume, ja esta no github? me explica o que foi feito e como, quero saber explicar e como eu mostro? a onde eiu vejo?
```

Resultado: a ferramenta encontrou e corrigiu erros na própria saída (seção 2.1).

### Prompt 5 — WhatsApp real e conferência

```
WhatsApp coloca o meu 35 999681545
sobre minha parte que eu tinha que fazer esta tudo certo? esta em formato humanizado? esta tudo coerente?
```

Resultado: o número real entrou no site. A ferramenta informou que a seção 3
ainda estava em branco e **se recusou a redigi-la**, porque ela precisa ser
escrita por mim.

### Prompt 6 — roteiro da revisão técnica

```
preciso que em pontos para revisao voce me liste os 3 mais faceis de fazer com explicacoes o codigo e um passo a passo de como fazer isso la, em que linha, qual parte etc
```

Resultado: a ferramenta indicou três pontos e onde ficam no código. A execução
das alterações e as justificativas da seção 3 ficam a meu cargo.

### Envio por engano (desconsiderado)

Mandei duas imagens sem relação com o projeto e, quando a ferramenta perguntou o
que fazer com elas, respondi:

```
MANDEI ERRADO DESCONSIDERE, esqueça elas
```

### Prompt 7 — repositório no GitHub

```
voce ja nao subiu no meu github? crie o repo como scallaseller-projetointegrador algo assim
```

Resultado: a ferramenta informou que não consegue criar repositórios na minha
conta. Eu criei o repositório vazio no GitHub.

### Prompt 8

```
Criei
```

Resultado: a ferramenta enviou as branches `entrega-1` e `main` para o
repositório.

### Prompt 9

```
pronto, agora o que eu faco, me explique o codigo, como foi feito e como estao as coisas que eram partes minha?
```

Resultado: explicação do código, página por página, e situação das minhas
tarefas.

### Prompt 10

*(apenas uma captura de tela, sem texto: a página de erro 404 do GitHub Pages,
"There isn't a GitHub Pages site here")*

Resultado: a ferramenta confirmou pela API do GitHub que o Pages ainda não
estava ativado e passou o passo a passo para ativar.

### Prompt 11

```
preciso que recapitule comigo, estou perdido. O que eu vou ter que fazer, como eu envio pra ele? como ficou a documentacao? inventou um prompt que eu te mandei?
```

Resultado: a ferramenta conferiu os prompts deste registro contra as minhas
mensagens. Nenhum tinha sido inventado. Ela completou os que faltavam, deixou
o texto exatamente como enviei e retirou duas frases que davam como feitas
alterações que eu ainda não tinha feito.

### Contexto adicional fornecido

Além dos prompts, a ferramenta usou dados da empresa que eu já tinha passado em
conversas anteriores. São os itens listados como "dados fornecidos por mim" na
seção 1.

**Até a data deste registro, nenhum outro prompt foi utilizado nesta entrega.**

---

## 2.1 Correções feitas pela própria IA (prompts 4 e 5)

> Estas correções foram feitas pela ferramenta na própria saída dela, depois dos
> meus pedidos de revisão. **Não fazem parte da minha revisão técnica**, que está
> na seção 3. Registro aqui por transparência: elas fazem parte do processo de
> uso da IA.

| # | Erro na versão gerada | Correção |
|---|---|---|
| 1 | O formulário usava `method="post"`. O GitHub Pages recusa POST e devolve erro 405 | `method` ficou no padrão (GET) até existir back-end |
| 2 | Comentário afirmava que um `<h3>` dentro do `<summary>` coloca a pergunta na lista de títulos. Vários leitores de tela tratam o `<summary>` como botão e descartam a semântica do heading | `<h3>` removido do `<summary>` e comentário corrigido |
| 3 | O WhatsApp de exemplo tinha DDD 35 e podia ser o número de uma pessoa real | Trocado por um número de DDD 00, que não existe |
| 4 | O texto inventava compromissos comerciais que eu nunca defini: diagnóstico gratuito, resposta em 1 dia útil, resultado em 3 a 6 meses, atendimento aos sábados, estruturação como pré-requisito, preço travado no anual | Removidos ou trocados por texto neutro |
| 5 | Atribuía ao meu sócio responsabilidades que eu nunca descrevi | Trocado por "Sócio-fundador", até eu definir os papéis |
| 6 | Legenda do painel dava a entender que era resultado real de cliente | Identificado como ilustrativo, com números fictícios |
| 7 | O método 360 tinha 6 frentes, mas o que eu passei tem 7 (Ads é uma frente separada) | Frente "Ads" adicionada |
| 8 | Texto das imagens sem acentuação ("Gestao", "Evolucao") | Imagens geradas de novo, com acento |
| 9 | Este registro listava arquivos que não existiam mais, não tinha os prompts 3 e 4 e afirmava que a IA não tinha participado do conteúdo de negócio | Registro reescrito |
| 10 | Cada pergunta do FAQ estava num `<article>` sem heading. O W3C acusava "Article lacks heading", sinal de over-tagging | O `<article>` passou a envolver o FAQ inteiro, que tem título próprio e faz sentido fora da página |
| 11 | A home ainda descrevia os canais com detalhes inventados ("Full", "programa de frete"), que já tinham saído da página Sobre | Texto da home igualado ao da página Sobre |
| 12 | O README citava uma seção "princípios" que não existia mais | README corrigido |

### Autoria dos commits

Os quatro primeiros commits da branch (`45ff434`, `1850cc4`, `37bb514`,
`f3a58f9`) foram criados pela ferramenta com o meu nome de usuário do git e
**sem** a marcação de coautoria. A partir do commit de correções, os commits
feitos pela IA trazem a linha `Co-Authored-By: Claude`, que o GitHub mostra como
coautor. Os commits da minha revisão técnica (seção 3) são só meus.

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
- **Script de verificação estrutural** — hierarquia de headings, âncoras
  quebradas, `alt` ausente, `label` órfão, `th` sem `scope`, `id` duplicado,
  `aria-current` incorreto e presença indevida de CSS/JS. Nenhuma falha.
