<div align="center">

# Registro de Uso de IA

**Projeto Integrador · Interface Web com HTML e CSS**
**Entrega 1 — Esqueleto Semântico** · branch `entrega-1`

</div>

| | |
|---|---|
| **Projeto** | Scalla Seller — site institucional de agência de marketplaces |
| **Aluno** | Gabriel Silva Machado · RA 98039075 · UNIVÁS, Sistemas de Informação |
| **Data** | 05/11/2026 |
| **Ferramentas de IA** | **Claude** (Anthropic): gerou e corrigiu o site e a primeira versão deste registro<br>**ChatGPT** (OpenAI): sugeriu melhorias de redação e organização deste registro |
| **Base** | Seção 5 do enunciado do Projeto Integrador |

**Conteúdo:** [1. Mapeamento de uso](#1-mapeamento-de-uso) · [2. O que a IA fez](#2-o-que-a-ia-fez) · [3. Revisão técnica](#3-revisão-técnica--alterações-feitas-por-mim) · [4. Validação](#4-validação-independente) · [Apêndice A. Prompts](#apêndice-a--prompts-na-íntegra)

## Resumo em 30 segundos

| | |
|---|---|
| 🤖 **A IA fez** | As 4 páginas HTML, as imagens provisórias, o README e a primeira versão deste registro |
| 👤 **Eu fiz** | Os dados reais da empresa, a decisão do tema, a conferência do que foi gerado e **3 alterações no código**, cada uma com a minha justificativa (seção 3) |
| ✅ **Verificado** | W3C Nu HTML Checker sem erros nas 4 páginas, depois das minhas alterações (seção 4) |

---

## 1. Mapeamento de uso

### 1.1 Código e arquivos

| Arquivo ou atividade | Participação da IA | Observação |
|---|:---:|---|
| `index.html`, `catalogo.html`, `sobre.html`, `contato.html` | **Integral** | Estrutura e redação geradas a partir do meu briefing |
| `img/*.png` | **Integral** | Imagens provisórias geradas por script Python (Pillow) |
| `README.md` | **Integral** | Gerado e corrigido pela IA |
| Este registro (seções 1, 2 e 4) | **Integral** | Escritas pelo Claude; o ChatGPT sugeriu depois melhorias de redação e organização |
| Pontos de revisão | **Integral** | A IA apontou pontos discutíveis no próprio código e onde alterar (prompt 6) |
| **Alterações da revisão técnica** | **Nenhuma** | Feitas por mim, direto no código, em commits meus |
| **Seção 3 deste registro** | **Nenhuma** | Justificativas escritas por mim |

### 1.2 Origem do conteúdo do site

A distinção entre **fatos** (meus) e **redação** (da IA) importa, por isso fica separada.

**Fatos fornecidos por mim (informação real da empresa)**

- Nome da agência, sócios e paleta azul e branco.
- Os dois serviços (estruturação e gestão mensal) e as 7 frentes do acompanhamento 360: onboarding, pesquisa de mercado, precificação, anúncios, criativos, Ads e gestão contínua.
- Canais: Mercado Livre e Shopee; TikTok Shop fora do escopo atual.
- Todos os preços das tabelas.
- Condições: sem limite de SKUs; verba de Ads paga pelo cliente.
- Público: CNPJ de qualquer nicho, já vendendo ou começando.
- WhatsApp de contato: (35) 99968-1545.

**Redigido pela IA, a confirmar por mim antes de o site ir ao ar de verdade**

- Todo o texto corrido (a redação das frases, não os fatos acima).
- O detalhamento das listas "O que entra" de cada serviço, no catálogo.
- Localização em Borda da Mata e horário de segunda a sexta, das 8h às 18h.
- Relatório mensal de acompanhamento para o cliente.
- Itens de "O que não está incluso" além da verba de Ads (logística, estoque e atendimento ao comprador final).

**Provisório ou fictício, já identificado como tal**

| Item | Situação |
|---|---|
| Painel com R$ 184 mil, 2.431 pedidos e ACOS de 9,4% | Números **fictícios**, avisados na própria página |
| `contato@scallaseller.com.br` | E-mail de exemplo, até a agência ter o endereço oficial |

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

### 2.1 Correções feitas pela própria IA (prompts 4 e 5)

> Feitas pela ferramenta na própria saída, depois dos meus pedidos de revisão.
> **Não fazem parte da minha revisão técnica** (seção 3).

| # | Onde | Problema na versão gerada | Correção |
|:-:|---|---|---|
| 1 | `contato.html` | Formulário com `method="post"`: o GitHub Pages recusa POST (erro 405) | `method` no padrão (GET) até haver back-end |
| 2 | `contato.html` | Comentário errado sobre `<h3>` dentro de `<summary>` | `<h3>` removido e comentário corrigido |
| 3 | `contato.html` | WhatsApp de exemplo que podia ser de uma pessoa real | Trocado por número fictício e, depois, pelo meu número real |
| 4 | Todas as páginas | Compromissos comerciais e funções do sócio inventados pela IA (prazo de resposta, diagnóstico grátis, atendimento aos sábados etc.) | Removidos ou trocados por texto neutro |
| 5 | `index.html` | Legenda do painel parecia resultado real de cliente | Marcado como ilustrativo, com números fictícios |
| 6 | `sobre.html` | Método 360 com 6 frentes em vez de 7 | Frente "Ads" adicionada |
| 7 | `img/` | Imagens sem acento ("Gestao", "Evolucao") | Imagens geradas de novo |
| 8 | `contato.html` | Cada pergunta do FAQ num `<article>` sem heading (W3C: "Article lacks heading") | Um único `<article>` envolvendo o FAQ |
| 9 | `index.html`, `README.md` | Detalhes inventados ou desatualizados | Textos igualados à página Sobre |

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

Além da revisão manual, o código passou por verificação automatizada.

| Verificação | Escopo | Resultado |
|---|---|---|
| **W3C Nu HTML Checker** (`vnu.jar`) | As 4 páginas | *"Document checking completed. No errors found."* Só um aviso informativo, sobre o suporte do atributo `inputmode` em navegadores antigos |
| **W3C Nu HTML Checker**, nova rodada depois das minhas 3 alterações (05/11/2026) | As 4 páginas | *"No errors found"*, com o mesmo aviso informativo |
| **Script de verificação estrutural** | Hierarquia de headings, âncoras quebradas, `alt` ausente, `label` órfão, `th` sem `scope`, `id` duplicado, `aria-current` incorreto e presença indevida de CSS ou JS | Nenhuma falha |
| **Teste de navegação por teclado** | Skip link, ordem do Tab e validação nativa do formulário | Funcionando |

> Essas verificações automatizadas não substituem a revisão manual de acessibilidade nem a minha revisão técnica (seção 3).

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

### Prompts seguintes

> A coluna **"Em resumo"** é uma síntese minha, só para facilitar a leitura. O que vale como registro é a coluna **"Texto original"**, copiada sem correção.

| # | Em resumo, eu pedi | Texto original (como enviei) | Resultado |
|:-:|---|---|---|
| 2 | Escolher o tema do site | Cliquei na opção oferecida pela ferramenta: `Scalla Seller — agência de marketplaces` | Tema definido |
| 3 | Ajustar o site ao modelo de tema do enunciado | `faça com que entre na sugestão do tema, dentro do que ele propôs` | Site reorganizado para a sugestão 2 (pequeno negócio local) |
| 4 | Revisar o código, corrigir erros e me explicar para eu saber apresentar | `QUERO QUE REVISE E PROCURE ERROS E Arrume, ja esta no github? me explica o que foi feito e como, quero saber explicar e como eu mostro? a onde eiu vejo?` | Erros corrigidos (seção 2.1) |
| 5 | Usar meu WhatsApp real e conferir a minha parte | `WhatsApp coloca o meu 35 999681545`<br>`sobre minha parte que eu tinha que fazer esta tudo certo? esta em formato humanizado? esta tudo coerente?` | Número aplicado; a IA não redigiu a seção 3 |
| 6 | Listar os 3 pontos mais fáceis para eu revisar, com o passo a passo | `preciso que em pontos para revisao voce me liste os 3 mais faceis de fazer com explicacoes o codigo e um passo a passo de como fazer isso la, em que linha, qual parte etc` | Três pontos indicados, com a localização |
| — | Ignorar duas imagens enviadas por engano | `MANDEI ERRADO DESCONSIDERE, esqueça elas` | Desconsideradas |
| 7 | Subir o projeto para o meu GitHub | `voce ja nao subiu no meu github? crie o repo como scallaseller-projetointegrador algo assim` | A IA não cria repositórios na minha conta; criei o vazio |
| 8 | Avisar que o repositório estava criado | `Criei` | Branches `entrega-1` e `main` enviadas |
| 9 | Entender o código e o que era parte minha | `pronto, agora o que eu faco, me explique o codigo, como foi feito e como estao as coisas que eram partes minha?` | Código explicado página por página |
| 10 | Mostrar o erro do GitHub Pages | Apenas uma captura de tela (404 do Pages), sem texto | Pages não estava ativo; passo a passo para ativar |
| 11 | Recapitular o que faltava e conferir se a IA inventou prompts | `preciso que recapitule comigo, estou perdido. O que eu vou ter que fazer, como eu envio pra ele? como ficou a documentacao? inventou um prompt que eu te mandei?` | Registro conferido contra as minhas mensagens |

### Prompts ao ChatGPT (melhoria deste registro)

| # | Em resumo, eu pedi | Texto original (como enviei) | Resultado |
|:-:|---|---|---|
| 12 | Melhorar o registro e manter anotado o que a IA fez | `melhore isso e faca um prompt paranque eu coloque em registro ia e deixe ainda o que ela fez anotado` | Depois enviei o registro como material |
| 13 | Esclarecer que a IA devia melhorar o que eu escrevi | `voce que vai fazer, to falando pra melhorar as coisas que eu escrevi etc` | Sugestões de redação e organização; sem mexer no código nem na seção 3 |

> **Pendente de completar:** os prompts em que pedi ao Claude orientação sobre as alterações da revisão técnica serão acrescentados aqui, com o texto exato, antes da entrega.

---

## Declaração

Declaro que este registro descreve o uso de ferramentas de IA nesta entrega conforme o histórico acima: o que foi gerado por IA, o que foi fornecido por mim e o que fiz sozinho. Pontos ainda pendentes estão sinalizados no próprio documento.

**Gabriel Silva Machado** · RA 98039075 · 05/11/2026
