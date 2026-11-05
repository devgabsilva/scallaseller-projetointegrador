Registro de Uso de IA — Entrega 1
Projeto: Scalla Seller — site institucional de agência de marketplaces
Aluno: Gabriel Silva Machado — RA 98039075
Entrega: 1 — Esqueleto Semântico (entrega-1)
Data do registro e desta revisão: 05/11/2026
Situação: documentação revisada; revisão técnica pessoal do aluno pendente de preenchimento.

Ferramentas utilizadas:
- Claude (Anthropic): geração inicial dos arquivos, revisões de código e apoio à documentação, conforme o histórico apresentado neste registro. Os modelos foram informados no documento original como “Opus 5” e “Opus 5.5”; essa identificação não foi conferida nesta revisão.
- ChatGPT (OpenAI): revisão da redação, organização e coerência deste documento em 05/11/2026. A participação desta ferramenta está detalhada na seção 5.
Este documento registra a participação das ferramentas de IA no desenvolvimento da entrega e distingue o conteúdo gerado, as informações fornecidas pelo aluno e as atividades que ainda dependem de execução pessoal. O documento original relaciona este registro à seção 5 do enunciado do Projeto Integrador.
1. Mapeamento do uso de IA
1.1. Código, imagens e documentação
O quadro abaixo reúne as informações do registro original e a revisão documental realizada nesta conversa. As implementações e os resultados técnicos anteriores foram relatados no material enviado pelo aluno; o repositório não foi inspecionado nesta revisão.
Arquivo ou atividade	Participação da IA	Participação do aluno e situação
index.html	Geração integral da versão inicial da estrutura e da redação	Briefing e informações da empresa fornecidos pelo aluno
catalogo.html	Geração integral da versão inicial da estrutura e da redação	Briefing e informações da empresa fornecidos pelo aluno
sobre.html	Geração integral da versão inicial da estrutura e da redação	Briefing e informações da empresa fornecidos pelo aluno
contato.html	Geração integral da versão inicial da estrutura e da redação	Dados de contato fornecidos pelo aluno
img/*.png	Geração de imagens provisórias por script Python com Pillow	Substituição por materiais definitivos ainda sujeita à definição do aluno
README.md	Geração inicial e correções documentais	Conferência final pelo aluno
Este registro	Geração inicial das seções documentais com Claude e revisão posterior de redação e organização com ChatGPT	Histórico e documento fornecidos pelo aluno
Identificação dos pontos de revisão	Claude apontou problemas discutíveis no código e preparou orientações a partir do prompt 6	Cabe ao aluno avaliar e escolher as alterações
Alterações da revisão técnica pessoal	Não há execução comprovada no material enviado	Pendentes de implementação e documentação pelo aluno
Seção 3 — justificativas pessoais	Não foram redigidas nesta revisão; somente o modelo de preenchimento foi organizado	Pendentes de redação pelo aluno, após as alterações reais


As correções executadas pela própria IA estão registradas na seção 2.1. Elas não são apresentadas como alterações pessoais do aluno.
1.2. Origem das informações do site
Informações fornecidas pelo aluno
Conforme o registro original, as seguintes informações vieram do aluno:
- Nome da agência, identificação dos sócios e paleta de cores azul e branco.
- Dois serviços: estruturação e gestão mensal de marketplaces.
- Sete frentes do acompanhamento 360: onboarding, pesquisa de mercado, precificação, anúncios, criativos, Ads e gestão contínua.
- Canais atendidos: Mercado Livre e Shopee. TikTok Shop está fora do escopo atual.
- Preços apresentados nas tabelas.
- Condições comerciais: ausência de limite de SKUs e verba de Ads paga pelo cliente.
- Público atendido: empresas com CNPJ, de qualquer nicho, que já vendem ou estão começando.
- WhatsApp de contato: (35) 99968-1545.
Conteúdo elaborado pela IA
A IA redigiu o texto corrido das páginas com base no briefing. A origem dos fatos fornecidos pelo aluno é distinta da autoria das frases usadas para apresentá-los.

Os itens abaixo foram incluídos pela IA e permanecem sujeitos à confirmação do aluno antes de uma publicação comercial:
- Detalhamento das listas “O que entra” de cada serviço no catálogo.
- Localização em Borda da Mata e atendimento de segunda a sexta-feira, das 8h às 18h.
- Oferta de relatório mensal de acompanhamento.
- Itens de “O que não está incluso” além da verba de Ads: logística, estoque e atendimento ao comprador final.
- Redação final das descrições e demais textos do site.
Dois conteúdos exigem identificação explícita:
Conteúdo	Situação registrada
Painel com R$ 184 mil, 2.431 pedidos e ACOS de 9,4%	Números fictícios de um painel ilustrativo. Segundo o registro original, essa condição está indicada na página.
contato@scallaseller.com.br	E-mail provisório usado como exemplo; não foi apresentado como endereço oficial confirmado.


2. Histórico de prompts e interações
Os prompts 1 a 11 abaixo foram transcritos do documento fornecido pelo aluno. A redação, os erros de digitação e as quebras de linha internas dos blocos foram mantidos conforme essa transcrição; foram removidos apenas os escapes de formatação presentes na cópia do documento. A correspondência com o histórico original do Claude não foi verificada nesta revisão.

As descrições de contexto e os parágrafos iniciados por Resultado ficam fora dos blocos: são explicações do processo e não fazem parte dos prompts.
Prompt 1 — Briefing inicial
Contexto informado: PDF do enunciado anexado à conversa.
[Projeto Integrador](https://www.ead.univas.edu.br/pluginfile.php/206109/mod_assign/intro/Projeto%20Integrador.pdf)
O que deve ter nesta entrega:
As 4 páginas em HTML puro, sem CSS:
Estrutura, semântica, hierarquia de headings, navegação interna funcional e checklist de acessibilidade aplicado.
Formato de Entrega
Enviar o link do repositório [GitHub](https://github.com/), a entrega deve corresponder a uma branch ou tag específica no repositório, para esta entrega use o nome da branch como entrega-1


LEIA O CONTEXTO E FACA
Interação 2 — Escolha do tema
Esta interação ocorreu por seleção de uma opção oferecida pela ferramenta, e não por um texto digitado pelo aluno. A opção escolhida foi:
Scalla Seller — agência de marketplaces
Prompt 3 — Adequação ao tema proposto
faça com que entre na sugestão do tema, dentro do que ele propôs
Resultado relatado: a primeira versão continha Home, Serviços, Planos e Contato. Após o pedido, a ferramenta reorganizou o site para a sugestão 2, descrita no registro como “site de pequeno negócio local”, com Home, Catálogo, Sobre e Contato. Localização e horários passaram a integrar a página de contato.
Prompt 4 — Revisão de erros e explicação da entrega
QUERO QUE REVISE E PROCURE ERROS E Arrume, ja esta no github? me explica o que foi feito e como, quero saber explicar e como eu mostro? a onde eiu vejo?
Resultado relatado: a ferramenta revisou a própria saída e corrigiu problemas. As correções informadas estão reunidas na seção 2.1.
Prompt 5 — Inclusão do WhatsApp e conferência das pendências
WhatsApp coloca o meu 35 999681545
sobre minha parte que eu tinha que fazer esta tudo certo? esta em formato humanizado? esta tudo coerente?
Resultado relatado: o WhatsApp real foi incluído no site. A ferramenta informou que a seção 3 ainda estava em branco e não a redigiu, por corresponder à revisão e às justificativas pessoais do aluno.
Prompt 6 — Orientações para a revisão técnica
preciso que em pontos para revisao voce me liste os 3 mais faceis de fazer com explicacoes o codigo e um passo a passo de como fazer isso la, em que linha, qual parte etc
Resultado relatado: a ferramenta indicou três pontos de revisão e sua localização no código. A implementação das alterações e a redação das justificativas permaneceram a cargo do aluno.
Envio por engano — Desconsiderado
O aluno enviou duas imagens sem relação com o projeto. Quando a ferramenta perguntou como utilizá-las, respondeu:
MANDEI ERRADO DESCONSIDERE, esqueça elas
O envio foi registrado como desconsiderado e não integra o conteúdo do site.
Prompt 7 — Criação do repositório
voce ja nao subiu no meu github? crie o repo como scallaseller-projetointegrador algo assim
Resultado relatado: a ferramenta informou que não poderia criar o repositório na conta do aluno. O aluno criou o repositório vazio no GitHub.
Prompt 8 — Confirmação da criação
Criei
Resultado relatado: a ferramenta enviou as branches entrega-1 e main para o repositório.
Prompt 9 — Explicação do código e das tarefas pessoais
pronto, agora o que eu faco, me explique o codigo, como foi feito e como estao as coisas que eram partes minha?
Resultado relatado: a ferramenta explicou o código de cada página e apresentou a situação das tarefas pessoais do aluno.
Interação 10 — Erro no GitHub Pages
Entrada informada: apenas uma captura de tela, sem texto, mostrando a mensagem de erro 404 do GitHub Pages: “There isn't a GitHub Pages site here”.

Resultado relatado: a ferramenta consultou a API do GitHub, identificou que o Pages ainda não estava ativado e orientou sua configuração. Esse relato não comprova, por si só, que a ativação foi concluída.
Prompt 11 — Recapitulação e conferência do histórico
preciso que recapitule comigo, estou perdido. O que eu vou ter que fazer, como eu envio pra ele? como ficou a documentacao? inventou um prompt que eu te mandei?
Resultado relatado: a ferramenta informou ter conferido o registro com as mensagens do aluno. Completou os prompts ausentes, preservou sua redação e retirou duas frases que apresentavam como concluídas alterações ainda não realizadas. A conferência é relatada aqui como parte do histórico anterior; não foi repetida pelo ChatGPT.
Contexto adicional utilizado pelo Claude
Segundo o registro original, a ferramenta também utilizou informações da empresa fornecidas pelo aluno em conversas anteriores. Esses dados estão relacionados na seção 1.2.
Prompt 12 — Pedido de melhoria documental ao ChatGPT
melhore isso e faca um prompt paranque eu coloque em registro ia e deixe ainda o que ela fez anotado
Contexto adicional: na mensagem seguinte, o aluno enviou o conteúdo integral do registro anterior como material para revisão.
Prompt 13 — Esclarecimento do pedido ao ChatGPT
voce que vai fazer, to falando pra melhorar as coisas que eu escrevi etc
Resultado dos prompts 12 e 13: o ChatGPT revisou a redação e a organização deste documento, corrigiu problemas de formatação e ajustou afirmações de autoria e conclusão de atividades. Os prompts históricos foram preservados conforme a transcrição recebida. As justificativas pessoais da seção 3 permaneceram pendentes. As mudanças documentais estão discriminadas na seção 5.
2.1. Correções de código e documentação atribuídas ao Claude
O registro anterior relaciona as correções abaixo aos pedidos de revisão, principalmente aos prompts 4 e 5. Elas fazem parte do trabalho da IA e não substituem a revisão técnica pessoal do aluno.
Nº	Problema registrado na versão anterior	Correção relatada
1	O formulário utilizava method="post", incompatível com o processamento pretendido na hospedagem estática do GitHub Pages.	O método passou a usar o padrão GET enquanto não houver back-end. Essa alteração não implementa o envio real de mensagens.
2	Um comentário afirmava que um <h3> dentro de <summary> garantiria a inclusão da pergunta na lista de títulos de leitores de tela.	O <h3> foi removido de <summary> e o comentário foi corrigido para não prometer esse comportamento.
3	O WhatsApp de exemplo utilizava DDD 35 e poderia corresponder ao contato real de outra pessoa.	Foi usado temporariamente um número com DDD 00. Depois, o prompt 5 solicitou a substituição pelo WhatsApp real do aluno.
4	O texto incluía compromissos comerciais não definidos pelo aluno: diagnóstico gratuito, resposta em um dia útil, resultados em três a seis meses, atendimento aos sábados, estruturação como pré-requisito e preço fixo no plano anual.	As afirmações foram removidas ou substituídas por formulações neutras.
5	O texto atribuía responsabilidades ao sócio sem que elas tivessem sido informadas.	A identificação foi reduzida a “Sócio-fundador”, até a definição dos papéis.
6	A legenda do painel poderia sugerir resultados reais de clientes.	O painel passou a ser identificado como ilustrativo, com números fictícios.
7	O acompanhamento 360 apresentava seis frentes, embora o briefing informasse sete.	A frente de Ads foi incluída separadamente.
8	As imagens continham palavras sem acentuação, como “Gestao” e “Evolucao”.	As imagens foram geradas novamente com os acentos.
9	O registro mencionava arquivos que já não existiam, omitia os prompts 3 e 4 e negava a participação da IA na elaboração do conteúdo de negócio.	O registro foi reescrito para refletir a participação informada.
10	Cada pergunta do FAQ estava em um <article> sem título, situação que gerava o aviso “Article lacks heading”, segundo a validação relatada.	O <article> passou a envolver o FAQ completo, que possui título próprio.
11	A página inicial ainda citava detalhes de canais não fornecidos pelo aluno, como “Full” e “programa de frete”.	O texto foi alinhado ao conteúdo da página Sobre.
12	O README mencionava uma seção “princípios” que já não existia.	A referência foi corrigida.


Autoria dos commits
Segundo o registro anterior, os quatro primeiros commits da branch — 45ff434, 1850cc4, 37bb514 e f3a58f9 — foram criados pela ferramenta com o nome de usuário configurado no Git, sem indicação de coautoria.

O mesmo registro informa que os commits posteriores de correção passaram a incluir uma indicação Co-Authored-By: Claude. A forma completa desse campo e sua associação no GitHub precisam ser conferidas no histórico do repositório; não foram verificadas nesta revisão documental.

Os commits da revisão técnica pessoal só deverão ser apresentados como realizados pelo aluno após a execução efetiva dessas alterações. O nome configurado como autor de um commit, isoladamente, não descreve toda a participação da IA no processo.
3. Revisão técnica — Alterações realizadas pelo aluno
Situação: pendente. O documento recebido não contém os trechos de código alterados nem as justificativas pessoais. Por isso, esta revisão organizou somente o modelo de preenchimento.

Conforme a orientação reproduzida no registro original, o aluno deverá selecionar pelo menos três pontos de PONTOS-PARA-REVISAO.md, avaliar o código, implementar as alterações e documentar sua decisão. Cada alteração deverá ter seu próprio commit, conforme o procedimento descrito no material enviado.

As explicações abaixo deverão ser escritas pelo aluno a partir do que realmente foi feito. Se houver apoio adicional de IA nessa etapa, sua participação também deverá ser registrada.
Alteração 1 — [Preencher o título]
Situação: pendente.
Arquivo e trecho: [Preencher após localizar o código.]
Commit: [Preencher após implementar a alteração.]

O que a IA gerou:
<!-- Inserir o trecho original. -->
O que foi alterado pelo aluno:
<!-- Inserir o trecho após a alteração. -->
Por que foi alterado:

[Explicar, com suas próprias palavras, o problema identificado e o motivo da solução escolhida.]

Como a alteração foi conferida:

[Descrever a verificação efetivamente realizada e o resultado observado.]
Alteração 2 — [Preencher o título]
Situação: pendente.
Arquivo e trecho: [Preencher após localizar o código.]
Commit: [Preencher após implementar a alteração.]

O que a IA gerou:
<!-- Inserir o trecho original. -->
O que foi alterado pelo aluno:
<!-- Inserir o trecho após a alteração. -->
Por que foi alterado:

[Explicar, com suas próprias palavras, o problema identificado e o motivo da solução escolhida.]

Como a alteração foi conferida:

[Descrever a verificação efetivamente realizada e o resultado observado.]
Alteração 3 — [Preencher o título]
Situação: pendente.
Arquivo e trecho: [Preencher após localizar o código.]
Commit: [Preencher após implementar a alteração.]

O que a IA gerou:
<!-- Inserir o trecho original. -->
O que foi alterado pelo aluno:
<!-- Inserir o trecho após a alteração. -->
Por que foi alterado:

[Explicar, com suas próprias palavras, o problema identificado e o motivo da solução escolhida.]

Como a alteração foi conferida:

[Descrever a verificação efetivamente realizada e o resultado observado.]
4. Validações automatizadas relatadas
O documento original informa a realização das verificações abaixo. Os resultados se referem à versão examinada naquela etapa. Não houve nova execução de validadores nem inspeção dos arquivos HTML nesta revisão com ChatGPT.
Verificação	Escopo informado	Resultado registrado anteriormente
W3C Nu HTML Checker (vnu.jar)	As quatro páginas HTML	“Document checking completed. No errors found.” O registro menciona ainda um aviso sobre o atributo inputmode; a mensagem completa e a versão do validador não foram fornecidas nesta conversa.
Script de verificação estrutural	Hierarquia de headings, âncoras quebradas, ausência de alt, labels órfãos, <th> sem scope, IDs duplicados, uso incorreto de aria-current e presença indevida de CSS ou JavaScript	Nenhuma falha, conforme o registro anterior.


Esses resultados documentam verificações automatizadas; não constituem, isoladamente, comprovação de acessibilidade completa ou de revisão técnica pessoal. Após as alterações do aluno, os resultados deverão ser atualizados com base na nova versão efetivamente verificada.
