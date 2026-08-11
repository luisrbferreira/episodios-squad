# Episódios Squad

Duas skills para Claude Code que transformam os bastidores de um evento ou lançamento numa **série documental em Reels** que gera desejo e vende, sem parecer anúncio.

O formato é um reality: o expert assume publicamente um desafio real com prazo ("será que dá pra lotar meu primeiro evento só produzindo conteúdo?") e documenta a jornada até o desfecho, episódio a episódio.

---

## De onde veio

Engenharia reversa da série da **[Jennifer Setti](https://instagram.com/jennifersetti)**, que lotou a primeira edição do evento presencial dela (sold-out antes da série terminar), com 50% dos ingressos vendidos no dia da abertura. Cada episódio novo ainda reativava respostas de um disparo de WhatsApp feito semanas antes.

A análise foi feita episódio a episódio: transcrição dos áudios, contagem de cortes, mapeamento de cenas, estrutura de roteiro, copy e edição. A Jennifer cedeu também os roteiros originais dela, que estão em `references/roteiros-originais.md`.

Feito por **[Luis Ferreira](https://instagram.com/luisrbferreira)** para o mastermind **Master Outsider**, do **[Bruno Gomes](https://instagram.com/brunogomesig)**.

---

## As skills

### `/ep-serie` — planejar a série

Coleta o contexto (ou lê os documentos da pasta do projeto), define a aposta pública com prazo e gera o `PLANO_DA_SERIE.md`:

- a aposta e o arco de episódios
- mapa de ganchos abertos (o que abre em cada episódio, onde fecha)
- matéria-prima a captar e personagens recorrentes
- kit de produção (banco de takes, referência por episódio)
- integração com o funil que já existe, inclusive sincronizar com disparo de WhatsApp
- palavra-chave de comentário por episódio

### `/ep-roteiro` — escrever cada episódio

Lê o plano, pergunta o que aconteceu de verdade desde o último episódio e entrega o roteiro pronto pra gravar no celular:

- minutado bloco a bloco (90 a 110 segundos)
- falas-guia no tom do expert, para adaptar, não decorar
- shot list de b-roll (cenas, prints, objetos)
- texto na tela e cartelas
- legenda do post e palavra-chave de comentário
- checklist de captação

---

## A fórmula de cada episódio

| Bloco | Tempo | O que acontece |
|---|---|---|
| Cold open | 0-5s | Pergunta-hipótese que evolui a cada episódio e embute o prazo |
| Vinheta | 5-12s | "Esse é o episódio N da série onde a gente vai descobrir se..." |
| Recap | 12-20s | "No episódio anterior eu te contei que..." |
| Conflito real | 20-50s | Um problema verdadeiro do processo |
| Aula embutida | 40-55s | Por que essa estratégia está sendo usada |
| Prova | 50-60s | Número ou print concreto |
| Semente | 55-80s | Abre a curiosidade do próximo episódio |
| CTA suave | 80-90s | A data repetida. Sem "link na bio" |
| Cliffhanger | final | A última frase aponta pro próximo episódio |

Regra dos ganchos: cada episódio fecha um e abre outro, com saldo de curiosidade sempre positivo. O último episódio responde a pergunta que abriu a série.

---

## Instalação

**Opção 1: clonando este repositório**

```bash
git clone https://github.com/luisrbferreira/episodios-squad.git /tmp/episodios-squad \
  && mkdir -p ~/.claude/skills \
  && cp -r /tmp/episodios-squad/ep-serie /tmp/episodios-squad/ep-roteiro ~/.claude/skills/ \
  && rm -rf /tmp/episodios-squad \
  && echo "✅ 2 skills do Episódios Squad instaladas!"
```

**Opção 2: baixando os pacotes**

```bash
mkdir -p ~/.claude/skills && cd ~/.claude/skills && for s in ep-serie ep-roteiro; do curl -fsSL "https://master-outsider-luis-ferreira.vercel.app/episodios-squad/$s.zip" -o "$s.zip" && unzip -oq "$s.zip" && rm "$s.zip"; done && echo "✅ 2 skills do Episódios Squad instaladas!"
```

Depois reabra o Claude Code Desktop e rode `/ep-serie` na pasta do seu projeto.

Requisitos: [Claude Code](https://claude.ai/download) com conta claude.ai. As skills funcionam na arquitetura do Claude Code, não em outros modelos.

---

## Como usar

1. Abra (ou crie) a pasta do projeto do seu evento ou lançamento.
2. Rode `/ep-serie`. Responda o que ela perguntar. Sai o `PLANO_DA_SERIE.md`.
3. A cada episódio, rode `/ep-roteiro` contando o que aconteceu de verdade na semana.
4. Grave, publique, e siga até o desfecho.

Serve para evento presencial, imersão ou lançamento digital. O que não muda: um desafio real com data, conflito verdadeiro e nada de urgência inventada.

---

## Estrutura

```
ep-serie/
├── SKILL.md
└── references/
    ├── metodo.md               # o método completo
    ├── roteiros-originais.md   # roteiros escritos pela Jennifer + kit de produção
    └── transcricoes.md         # transcrições dos episódios
ep-roteiro/
└── (mesma estrutura)
```

---

## Créditos

- Estratégia, execução e roteiros originais: **Jennifer Setti** ([@jennifersetti](https://instagram.com/jennifersetti))
- Engenharia reversa, skills e empacotamento: **Luis Ferreira** ([@luisrbferreira](https://instagram.com/luisrbferreira))
- Mastermind onde tudo isso circulou primeiro: **Master Outsider**, do **Bruno Gomes** ([@brunogomesig](https://instagram.com/brunogomesig))

O material de referência é do case real e serve para modelar estrutura e ritmo. Não copie frases literais para outro perfil: adapte com as palavras de quem vai falar.
