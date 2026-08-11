---
name: ep-roteiro
description: Escreve o roteiro minutado do próximo episódio da sua Série de Episódios (reality de bastidores no Instagram), com falas-guia, shot list de b-roll, legendas, caption e palavra-chave de comentário. Parte do Episódios Squad do Master Outsider. Use SEMPRE que o usuário rodar /ep-roteiro ou pedir o roteiro de um episódio da série, "escrever o episódio 2", roteirizar bastidor da semana, ou variações. Funciona lendo o PLANO_DA_SERIE.md gerado pela skill /ep-serie (se não existir, colete o essencial ou sugira rodar /ep-serie primeiro).
---

# /ep-roteiro — Roteirizar o próximo episódio

Você vai escrever o roteiro de UM episódio da série documental do usuário, pronto pra gravar no celular: minutado, com falas-guia no tom dele, shot list e caption.

Antes de escrever, leia `references/metodo.md` (fórmula completa e princípios de copy) e `references/roteiros-originais.md` (os roteiros que a Jennifer escreveu antes de gravar: é o padrão de escrita a modelar, inclusive a legenda escrita junto do roteiro). Use `references/transcricoes.md` pra calibrar tom de fala.

## Passo 1 — Recuperar o contexto

1. Procure o `PLANO_DA_SERIE.md` na pasta do projeto (gerado por /ep-serie). Ele define a aposta, o arco, os loops e as palavras-chave.
   - Se não existir: pergunte se o usuário quer rodar /ep-serie primeiro (recomendado) ou, se ele preferir seguir direto, colete o mínimo: a aposta com prazo, número deste episódio, o que já foi contado antes.
2. Pergunte (uma coisa por vez, só o que faltar):
   - **O que aconteceu de verdade desde o último episódio?** (vitórias, perrengues, números novos, conversas, decisões). O episódio é feito de fato real, não de invenção.
   - Que provas/materiais existem dessa semana (prints, fotos, números)?
3. Confira no plano qual loop este episódio fecha e qual abre. Se a realidade mudou o arco (aconteceu algo melhor que o planejado), atualize o plano e use a realidade. O sold-out antecipado, o fornecedor que errou, a mensagem inesperada: isso É o episódio.

## Passo 2 — Escrever o roteiro

Estrutura obrigatória do episódio (90 a 110 segundos; a fórmula detalhada com exemplos está em `references/metodo.md`):

```
[0-5s]   COLD OPEN — pergunta-hipótese que evolui a cada episódio e embute o prazo
[5-12s]  VINHETA — "Esse é o episódio N da série onde a gente vai descobrir se [aposta]"
         (frase quase idêntica em todos os episódios: é a assinatura da série)
[12-20s] RECAP (do Ep2 em diante) — "No episódio anterior eu te contei que..."
[20-50s] CONFLITO REAL — um problema verdadeiro e específico do processo
[40-55s] AULA EMBUTIDA — o expert explica POR QUE está usando aquela estratégia
         (é o que transforma bastidor em autoridade)
[50-60s] PROVA — número/print concreto e verdadeiro
[55-80s] SEMENTE — abre um open loop novo pro próximo episódio
[80-90s] CTA SUAVE — a data/meta repetida 2x ao longo do episódio; proibido "link na bio"
[final]  CLIFFHANGER — última frase aponta pro próximo episódio, sempre
```

## Formato de saída (salvar como ROTEIRO_EP[N].md no projeto)

```markdown
## EPISÓDIO N — [título interno]
**Pergunta do cold open:** ...
**Loop que fecha:** ... | **Loop que abre:** ...
**Publicar em:** [data]

### Roteiro minutado
| Tempo | Fala-guia (adaptar ao seu jeito de falar) | Cena / b-roll | Texto na tela |
|---|---|---|---|
| 0-5s | ... | ... | ... |
[cobrir todos os blocos da fórmula]

### Caption do post
[continua a história, não resume o vídeo; fecha com pergunta + palavra-chave]

### Palavra-chave de comentário: [PALAVRA]

### Checklist de captação
- [ ] [cada cena/print/objeto que precisa ser gravado ou coletado]
```

## Se for o último episódio

O episódio final responde a pergunta-hipótese que abriu a série: a mesma pergunta do Ep1, agora com o resultado na mão. Entregue o resultado logo no início, sem enrolar, e feche o arco. Se o resultado ficou abaixo do esperado, conte com honestidade: quem acompanhou quer o desfecho de qualquer jeito, e a franqueza sustenta a próxima série.

## Regras que não se negociam

- **Falas-guia, não decoreba**: o expert fala com as palavras dele; marque as falas como adaptáveis. Tom de conversa de WhatsApp, com humor autodepreciativo leve (1-2 por episódio).
- **Só fato verdadeiro**: número, print e urgência apenas reais. "Faltam poucos ingressos" só quando for verdade. O próprio desfecho (bateu ou não bateu a meta) vira conteúdo, inclusive se der errado.
- **Anti-venda declarada**: em algum episódio o expert verbaliza o próprio mecanismo ("não vou te empurrar nada, vou te levar pros bastidores"). Dizer isso em voz alta É a venda.
- **B-roll prova cada frase**: cada afirmação da fala tem uma cena correspondente na shot list (print, objeto, espaço, reunião). 1 meme por episódio como respiro.
- **Mesmo look e paleta** da série inteira (continuidade de reality).
- Português do Brasil, sem travessão e sem reticências nas falas e captions.
