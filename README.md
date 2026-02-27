# Animated Star Button

Um botão interativo e moderno criado com **HTML5** e **CSS3**, apresentando uma animação de partículas (estrelas) que reage ao movimento do mouse (hover).

## Visual do Projeto

O botão possui um design minimalista com um fundo pêssego (`#fec195`). Ao passar o mouse, as estrelas que estão ocultas atrás do botão "explodem" para posições aleatórias com diferentes velocidades e trajetórias, criando um efeito dinâmico e fluido.

## Tecnologias Utilizadas

* **HTML5**: Estruturação semântica e SVGs inline para ícones vetoriais.
* **CSS3**: 
    * **Posicionamento Absoluto**: Para controlar a dispersão das estrelas.
    * **Cubic-bezier**: Para criar movimentos de aceleração e desaceleração orgânicos.
    * **Transitions & Filters**: Para efeitos de sombra (`drop-shadow`) e suavidade.
    * **Z-index**: Gerenciamento de camadas para esconder/mostrar elementos.

## Como o código funciona

### 1. Estrutura SVG
As estrelas são caminhos vetoriais (`path`) inseridos diretamente no HTML. Isso permite que elas sejam leves e escaláveis sem perder resolução.

### 2. Animação de Dispersão
Cada estrela possui uma classe individual (`.star-1` até `.star-6`). No estado inicial, elas estão centralizadas e atrás do botão. No estado `:hover`, cada uma recebe coordenadas de `top` e `left` diferentes:

| Estrela | Delay/Curva | Efeito de Saída |
| :--- | :--- | :--- |
| Star 1 | 1s (Bezier) | Sobe para a esquerda |
| Star 2 | 1s (Curva Lenta) | Move para o topo |
| Star 5 | 0.6s (Rápida) | Dispara para a direita |

### 3. Estilização do Botão
O botão utiliza `transition: all 0.3s ease-in-out` para garantir que a mudança de cor e o brilho (`box-shadow`) não sejam bruscos.

## Como clonar e testar

1. Clone o repositório:
   ```bash
   git clone [https://github.com/seu-usuario/nome-do-projeto.git](https://github.com/seu-usuario/nome-do-projeto.git)


  <img width="162" height="74" alt="image" src="https://github.com/user-attachments/assets/1db086e2-0318-44f2-89ba-85c6190ede28" />
