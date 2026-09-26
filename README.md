# 🥪 Sanduba

Um jogo de palavras diário em português, inspirado no [betweenle.com](https://betweenle.com/).

**[👉 Jogar agora](https://a-hanauer.github.io/sanduba-jogo/)**

## Como jogar

Existe um **recheio secreto de 5 letras** escondido em algum lugar de um dicionário
ordenado alfabeticamente — e ele está sempre entre duas fatias de pão.

A cada palpite de 5 letras que você envia, o jogo mostra se a palavra secreta vem
**antes** ou **depois** dele no dicionário. O palpite vira uma nova fatia em cima ou
embaixo, junto com uma pontuação fixa: quanto menor o número, mais perto do recheio
ele está. Essa escala não muda ao longo da partida, então dá pra comparar a distância
de qualquer palpite com qualquer outro.

Cada palpite estreita o intervalo até sobrar só a palavra secreta. Você tem
**14 tentativas** por partida.

- **Palavra do dia** — a mesma para todo mundo, muda à meia-noite local.
- **Jogo livre** — palavra aleatória, joga quantas vezes quiser (switch ao lado da engrenagem).

Você pode digitar qualquer palavra válida de 5 letras como palpite — inclusive
plurais, flexões de verbo e variações de gênero. Já a palavra secreta em si é sempre
sorteada só entre palavras "de dicionário" (sem plural nem flexão), pra não sair algo
impossível de adivinhar. Acentos também não atrapalham: digitar "c" aceita palavras
com "ç", "a" aceita "á"/"ã", e assim por diante.

## Rodando localmente

O jogo é um único arquivo HTML autocontido — sem build, sem dependências.

```bash
git clone https://github.com/a-hanauer/sanduba-jogo.git
cd sanduba-jogo
# abra index.html direto no navegador, ou sirva com qualquer servidor estático:
python3 -m http.server 8000
```

## Publicando no GitHub Pages

1. Faça upload do `index.html` para a raiz do repositório.
2. Em **Settings → Pages**, defina a branch `main` e a pasta `/ (root)`.
3. Aguarde a build e acesse o link gerado.

## Adicionar à tela de início (iOS/Android)

Abra o link no Safari (iOS) ou Chrome (Android), toque em **Compartilhar** →
**Adicionar à Tela de Início**. O jogo abre em tela cheia, como um app nativo.

## Dicionário

- **~3.200 palavras aceitas como palpite** — inclui plurais e flexões verbais comuns.
- **~2.240 palavras possíveis como segredo** — apenas formas de dicionário (sem
  plural, sem flexão), pra manter o jogo sempre solucionável.

Compilado a partir de listas públicas do [dicio.com.br](https://www.dicio.com.br/).

## Créditos

- Mecânica original: [betweenle.com](https://betweenle.com/)
- Ilustração do sanduíche: [OpenMoji](https://openmoji.org) — licenciada sob
  [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/). As cores foram
  adaptadas para a paleta do jogo; a versão adaptada segue sob a mesma licença.

## Licença

Código do jogo: sem licença definida ainda — adicione uma (MIT é uma opção comum
para projetos assim) se quiser deixar explícito o que outras pessoas podem fazer com ele.
