---
name: ep-serie
description: Planeja a sua Série de Episódios no Instagram (reality de bastidores que vende) para lotar evento presencial, imersão ou bater meta de lançamento documentando a jornada real. Parte do Episódios Squad do Master Outsider. Use SEMPRE que o usuário rodar /ep-serie ou pedir para planejar série de episódios, reels em episódios, documentar bastidores de evento ou lançamento, "fazer igual a estratégia de episódios", vender ingressos sem parecer vendedor, ou variações. Gera o PLANO_DA_SERIE.md que a skill /ep-roteiro usa depois para escrever cada episódio.
---

# /ep-serie — Planejar a Série de Episódios

Você vai montar o plano de uma série documental em Reels no formato **reality de bastidores**: o expert assume publicamente um desafio com prazo ("será que dá pra lotar meu primeiro evento só com conteúdo?") e documenta a jornada real, episódio a episódio, até o desfecho.

Formato validado em produção pela Jennifer Setti (@jennifersetti), no Master Outsider: primeiro evento presencial **sold-out antes da série terminar**, e cada episódio novo ainda reativava respostas de um disparo de WhatsApp feito semanas antes. Por que funciona: retenção de reality (pergunta-hipótese + cliffhanger) sem cara de anúncio; bastidor substitui prova social quando não há edições anteriores; vulnerabilidade real faz a audiência torcer em vez de fugir de venda.

Antes de gerar qualquer coisa, leia `references/metodo.md` (o método completo) e `references/roteiros-originais.md` (os roteiros reais da Jennifer e o kit de produção dela: banco de takes do espaço, vídeo de referência por episódio, legenda escrita junto do roteiro). Use `references/transcricoes.md` quando precisar calibrar tom de fala.

## Passo 1 — Contexto do usuário

Primeiro, procure contexto já existente: arquivos na pasta atual do projeto (briefings, `contexto/`, documentos do negócio, um `PLANO_DA_SERIE.md` anterior). Aproveite tudo que já estiver respondido.

O que você precisa saber (pergunte APENAS o que faltar, uma pergunta por vez, começando pela mais importante):

1. **O desafio com prazo**: o que está em jogo e até quando? (lotar evento até dd/mm, bater X vendas até dd/mm). Sem prazo real não existe série; ajude o usuário a formular a aposta se ele estiver vago.
2. **O produto**: evento/imersão/lançamento, nome, data, cidade (se presencial), promessa central, preço/lotes se houver.
3. **O momento da campanha**: já anunciou? já abriu vendas/lote? já fez disparo de WhatsApp pra base? tem palavras-chave de comentário rodando (ManyChat ou similar)?
4. **Matéria-prima real disponível**: espaço, reuniões, prints de WhatsApp, fornecedores, brindes, personagens do time (produtora, mentor, sócio), edições anteriores.
5. **Quantos episódios cabem** até o prazo (padrão: 4 a 6, com Ep1 e Ep2 em dias seguidos).

## Passo 2 — Gerar o PLANO_DA_SERIE.md

Salve um arquivo `PLANO_DA_SERIE.md` na pasta do projeto com exatamente estas seções:

```markdown
# Plano da Série — [nome da série]

## A aposta pública
[pergunta-hipótese central + prazo. Ex.: "Será que é possível lotar meu primeiro evento presencial só produzindo conteúdo?"]

## Contexto do negócio
[produto, data, promessa, momento da campanha, o que já existe de funil]

## Fundação de campanha
[Se o usuário JÁ tem funil rodando: como a série se sincroniza (episódio novo reativa
disparo antigo de WhatsApp; palavras-chave por peça). Se NÃO tem: o mínimo a montar
ANTES do Ep1 (anúncio da data + captura por palavra-chave de comentário) e por quê:
sem fundação a série entrega menos, ela é camada de reengajamento e reta final,
não substitui o funil.]

## Arco da série
[tabela: Ep | data de publicação | pergunta do cold open | conflito central | o que prova | loop que fecha | loop que abre]
[O ÚLTIMO episódio responde a pergunta-hipótese que abriu a série. Reserve-o pro
fechamento e defina quando soltar (no dia do evento, na virada da meta). Se o
resultado for negativo, o fechamento honesto também é episódio.]

## Mapa de open loops
[lista dos loops da série: onde abre, onde fecha. Regra: cada episódio fecha 1 e abre
outro; saldo de curiosidade sempre positivo; um loop pode atravessar episódios.]

## Matéria-prima e personagens
[o que gravar/coletar desde JÁ (o b-roll é o processo real): reuniões, prints,
objetos, espaço, bastidor da própria gravação; personagens recorrentes com nome]

## Kit de produção
[monte como no case: pasta de takes do espaço/processo gravados de uma vez e
reaproveitados; pasta de áudios; um vídeo de referência por episódio pra modelar
formato; roteiro e legenda no mesmo arquivo; documento vivo com o próximo episódio
já em escrita]

## Identidade visual da série
[mesmo look/figurino em todos os episódios, paleta da marca, tipografia das legendas,
cartelas de respiro, 1 meme por episódio]

## Palavras-chave por episódio
[uma palavra de comentário própria por episódio + o que o fluxo de DM entrega]

## Próximo passo
Rode /ep-roteiro para escrever o roteiro do Episódio 1.
```

## Regras que não se negociam

- **Aposta honesta**: o desafio é real e pode dar errado; é isso que gera a torcida. Nunca fabricar drama nem urgência falsa.
- **A série vende sem vender**: zero "link na bio", zero "corre que está acabando" sem ser verdade. O CTA é a data repetida e a palavra-chave de comentário.
- **Datas e números só verdadeiros**: prova é print real, número real. Se ainda não existe, o plano marca o placeholder e espera o fato acontecer.
- **Adaptar, não copiar**: o método vem de um caso de evento presencial, mas a aposta funciona para lançamento, desafio de meta, inauguração. O que não muda: pergunta-hipótese, prazo, conflito real, cliffhanger.
- Escreva tudo em português do Brasil, sem travessão e sem reticências nas falas e captions.
