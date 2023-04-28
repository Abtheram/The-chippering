# The-chippering
The chippering project
Game title: The chippering(The last tree) The purpose of the project is to give me a better understanding of what it takes to create the games I love to play. For the game I want to make a fun 2D shooter game that is level based and almost retro with how it plays. An old fashion level based shooter with a funny twist. To make this project ill be using python 3 and PYgame to help me create the fundementals of the game like images, sound affect, motion, backround, etc.




Helping to code the timer for the games https://www.youtube.com/watch?v=CJeElAsOvzc 
Backround for the py game https://www.askpython.com/python-modules/pygame-looping-background#:~:text=To%20add%20the%20background%20image,we%20will%20be%20using%20transform.
Backround: 
import pygame
from pygame.locals import *
pygame.init()
width = 1000
height = 500
window = pygame.display.set_mode((width,height))
bg_img = pygame.image.load('my image')
bg_img = pygame.transform.scale(bg_img,(width,height))
i = 0
runing = True
while runing:
    window.blit(bg_img,(i,0))
    i-=1
    for event in pygame.event.get():
        if event.type == QUIT:
            runing = False   
    pygame.display.update()
pygame.quit()
