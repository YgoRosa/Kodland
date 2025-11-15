# Jogo Kodland

Este é um jogo de plataforma simples criado com a biblioteca `pgzero`. O jogo apresenta um herói que pode pular e se mover horizontalmente, inimigos como abelhas, lesmas de fogo e cracas, e obstáculos.

## Características do Jogo

- **Mecânica de Plataforma**: O herói se move e salta em plataformas com física básica de gravidade.
- **Construção de Nível**: O mapa é construído a partir de arquivos CSV (`mapa_plataformas.csv`, `mapa_obstaculos.csv`, `mapa_personagem.csv`, `mapa_inimigos.csv`) que definem a posição das plataformas, obstáculos, do personagem e dos inimigos.
- **Inimigos**: O jogo inclui inimigos como abelhas (`bee`), lesmas de fogo (`slimefire`) e cracas (`barnacle`), cada um com suas próprias animações e comportamentos.
- **Obstáculos**: Existem obstáculos que, ao serem colididos, fazem o herói retornar à posição inicial.
- **Objetivo**: O herói precisa alcançar uma bandeira (`goal`) para completar o nível, o que também o leva de volta ao início.

## Como Jogar

1.  Certifique-se de ter o Python e a biblioteca `pgzero` instalados.
2.  Execute o arquivo `game.py` para iniciar o jogo.
3.  Use as teclas de seta (`left` e `right`) para mover o herói horizontalmente.
4.  Use a barra de espaço para pular.
5.  Evite os inimigos e obstáculos para não voltar para o começo.

## Sugestão para Resolução de Tela (Zoom)
O jogo foi projetado para uma grade de 30 x 15 tiles de 64 pixels cada, resultando em uma resolução de 1920 X 960 pixels.
Se o jogo parecer muito `zoomado` ou as bordas da janela ficarem fora da tela:
Isso pode ocorrer se a resolução nativa do seu monitor for menor que 1920 X 960 ou se o dimensionamento do seu sistema operacional (Windows/macOS) estiver ajustado para mais de 100%.
Para melhorar a visualização e evitar que o jogo fique com zoom excessivo, considere diminuir a resolução de tela do seu computador antes de executar o jogo.

## Estrutura do Repositório

- `game.py`: O código-fonte principal do jogo.
- `mapa.tmx`: Arquivo de mapa do Tiled, que define a estrutura visual do nível.
- `mapa_plataformas.csv`: Arquivo CSV que define a posição das plataformas.
- `mapa_obstaculos.csv`: Arquivo CSV que define a posição dos obstáculos.
- `mapa_personagem.csv`: Arquivo CSV que define a posição inicial do personagem.
- `mapa_inimigos.csv`: Arquivo CSV que define a posição dos inimigos.
- `spritesheet-tiles-default.tsx`: Arquivo de tileset Tiled que define os blocos usados no mapa.