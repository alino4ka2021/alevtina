# pin - pong
# мой проект пин_понг
#Персонажи из моей игры будут передвигаться. Мячик рандомно, корзины с помощью клавиш "вверх"  и "вниз" или "S", "W"
from pygame import *

back =  [200, 255, 255]
win_width = 700
win_height = 500
display.set_caption("Shooter")
window = display.set_mode((win_width, win_height))
window.fill(back)

clock = time.Clock()
FPS = 60
game = True

while game:
    for e in event.get():
        if e.type == QUIT:
            game = False


    display.update()
    clock.tick(FPS)
