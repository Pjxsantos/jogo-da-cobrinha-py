# jogo-da-cobrinha-py

1. **Instale o Pygame:** Primeiro, certifique-se de ter o Pygame instalado. Se ainda não o fez, instale-o usando o seguinte comando no terminal:
```yaml
   pip install pygame
```
 2. **Crie o esqueleto do jogo:** Vamos começar criando a estrutura básica do jogo. Crie um arquivo chamado snake_game.py e adicione o seguinte código:
```yaml
  import pygame
import sys

pygame.init()

# Defina as dimensões da tela
screen_width, screen_height = 640, 480
screen = pygame.display.set_mode((screen_width, screen_height))
pygame.display.set_caption("Snake Game")

# Loop principal do jogo
while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()

    # Atualize a tela
    pygame.display.flip()
```
3. **Adicione a cobrinha e a maçã:** Agora, vamos criar a cobrinha e a maçã. Adicione as classes Snake e Apple ao seu código. A cobrinha será representada por uma lista de segmentos, e a maçã será um retângulo vermelho.

4. **Lógica do jogo:**
A cobrinha se move continuamente na direção atual.
Se a cobrinha colidir com a parede ou consigo mesma, o jogo termina.
Quando a cobrinha come uma maçã, ela cresce e uma nova maçã aparece em uma posição aleatória.

5. **Controles:**
Use as teclas de seta para controlar a direção da cobrinha.

6. **Renderize a cobrinha e a maçã:**
Desenhe a cobrinha e a maçã na tela usando retângulos ou círculos.
Atualize a tela a cada quadro.

7. **Loop do jogo:**
Verifique colisões.
Atualize a posição da cobrinha.
Verifique se a cobrinha comeu a maçã.

8. **Pontuação:**
Mantenha a pontuação do jogador com base no número de maçãs comidas.

**Lembre-se de que este é apenas um esqueleto básico. Você pode expandir o jogo adicionando mais recursos, como placar, níveis de dificuldade e efeitos sonoros. Divirta-se criando seu próprio jogo da cobrinha! 🐍🍎**

