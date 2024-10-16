<p><strong>Chapter 15: Building a Simple Game</strong></p>

<p>In this chapter, we will explore the process of building a simple game using a programming language. We will use Python as our programming language of choice, and the Pygame library to create a game window and handle user input.</p>

<p><strong>Why Build a Game?</strong></p>

<p>Building a game can be a fun and rewarding experience, and it's a great way to practice your programming skills. Games can be complex and challenging to create, but they can also be simple and easy to understand. In this chapter, we will focus on building a simple game that demonstrates the basics of game development.</p>

<p><strong>What We Will Build</strong></p>

<p>In this chapter, we will build a simple game called "Pong." Pong is a classic game where two players control paddles and hit a ball back and forth on a screen. The game will have the following features:</p>

<ul>
<li>A game window with a black background</li>
<li>Two paddles that can be controlled by the player using the arrow keys</li>
<li>A ball that bounces off the edges of the screen and the paddles</li>
<li>A score that increments when a player misses the ball</li>
</ul>

<p><strong>Setting Up the Game</strong></p>

<p>To start building the game, we need to set up the game window and import the necessary libraries. We will use the Pygame library to create the game window and handle user input.</p>

<p>```python
import pygame
import sys</p>

<h1>Initialize Pygame</h1>

<p>pygame.init()</p>

<h1>Set up the game window</h1>

<p>screen<em>width = 800
screen</em>height = 600
screen = pygame.display.set<em>mode((screen</em>width, screen_height))</p>

<h1>Set up the title of the game window</h1>

<p>pygame.display.set_caption("Pong")</p>

<h1>Set up the font for the score</h1>

<p>font = pygame.font.Font(None, 36)
```</p>

<p><strong>Creating the Paddles</strong></p>

<p>Next, we need to create the paddles that will be controlled by the player. We will use two rectangles to represent the paddles.</p>

<p>```python</p>

<h1>Set up the paddles</h1>

<p>paddle<em>width = 10
paddle</em>height = 100
paddle_speed = 5</p>

<p>paddle1<em>x = 0
paddle1</em>y = screen<em>height / 2 - paddle</em>height / 2</p>

<p>paddle2<em>x = screen</em>width - paddle<em>width
paddle2</em>y = screen<em>height / 2 - paddle</em>height / 2
```</p>

<p><strong>Creating the Ball</strong></p>

<p>Next, we need to create the ball that will bounce off the edges of the screen and the paddles. We will use a circle to represent the ball.</p>

<p>```python</p>

<h1>Set up the ball</h1>

<p>ball<em>radius = 10
ball</em>speed<em>x = 5
ball</em>speed_y = 5</p>

<p>ball<em>x = screen</em>width / 2
ball<em>y = screen</em>height / 2
```</p>

<p><strong>Handling User Input</strong></p>

<p>Next, we need to handle user input to control the paddles. We will use the arrow keys to control the paddles.</p>

<p>```python</p>

<h1>Handle user input</h1>

<p>while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()</p>

<pre><code>keys = pygame.key.get_pressed()
if keys[pygame.K_UP]:
    paddle1_y -= paddle_speed
if keys[pygame.K_DOWN]:
    paddle1_y += paddle_speed
if keys[pygame.K_w]:
    paddle2_y -= paddle_speed
if keys[pygame.K_s]:
    paddle2_y += paddle_speed
</code></pre>

<p>```</p>

<p><strong>Updating the Game State</strong></p>

<p>Next, we need to update the game state based on the user input and the game logic. We will update the position of the ball and the paddles.</p>

<p>```python</p>

<h1>Update the game state</h1>

<p>ball<em>x += ball</em>speed<em>x
ball</em>y += ball<em>speed</em>y</p>

<p>if ball<em>y &lt; 0 or ball</em>y &gt; screen<em>height - ball</em>radius:
    ball<em>speed</em>y *= -1</p>

<p>if ball<em>x &lt; paddle1</em>x + paddle<em>width and ball</em>y &gt; paddle1<em>y and ball</em>y &lt; paddle1<em>y + paddle</em>height:
    ball<em>speed</em>x *= -1
if ball<em>x &gt; screen</em>width - paddle2<em>x - paddle</em>width and ball<em>y &gt; paddle2</em>y and ball<em>y &lt; paddle2</em>y + paddle<em>height:
    ball</em>speed_x *= -1
```</p>

<p><strong>Drawing the Game</strong></p>

<p>Finally, we need to draw the game on the screen. We will draw the paddles, the ball, and the score.</p>

<p>```python</p>

<h1>Draw the game</h1>

<p>screen.fill((0, 0, 0))
pygame.draw.rect(screen, (255, 255, 255), (paddle1<em>x, paddle1</em>y, paddle<em>width, paddle</em>height))
pygame.draw.rect(screen, (255, 255, 255), (paddle2<em>x, paddle2</em>y, paddle<em>width, paddle</em>height))
pygame.draw.circle(screen, (255, 255, 255), (int(ball<em>x), int(ball</em>y)), ball_radius)</p>

<p>score = font.render(str(score), True, (255, 255, 255))
screen.blit(score, (screen_width / 2, 10))</p>

<p>pygame.display.flip()
```</p>

<p><strong>Putting it All Together</strong></p>

<p>Here is the complete code for the game:</p>

<p>```python
import pygame
import sys</p>

<h1>Initialize Pygame</h1>

<p>pygame.init()</p>

<h1>Set up the game window</h1>

<p>screen<em>width = 800
screen</em>height = 600
screen = pygame.display.set<em>mode((screen</em>width, screen_height))</p>

<h1>Set up the title of the game window</h1>

<p>pygame.display.set_caption("Pong")</p>

<h1>Set up the font for the score</h1>

<p>font = pygame.font.Font(None, 36)</p>

<h1>Set up the paddles</h1>

<p>paddle<em>width = 10
paddle</em>height = 100
paddle_speed = 5</p>

<p>paddle1<em>x = 0
paddle1</em>y = screen<em>height / 2 - paddle</em>height / 2</p>

<p>paddle2<em>x = screen</em>width - paddle<em>width
paddle2</em>y = screen<em>height / 2 - paddle</em>height / 2</p>

<h1>Set up the ball</h1>

<p>ball<em>radius = 10
ball</em>speed<em>x = 5
ball</em>speed_y = 5</p>

<p>ball<em>x = screen</em>width / 2
ball<em>y = screen</em>height / 2</p>

<h1>Set up the score</h1>

<p>score = 0</p>

<h1>Handle user input</h1>

<p>while True:
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            pygame.quit()
            sys.exit()</p>

<pre><code>keys = pygame.key.get_pressed()
if keys[pygame.K_UP]:
    paddle1_y -= paddle_speed
if keys[pygame.K_DOWN]:
    paddle1_y += paddle_speed
if keys[pygame.K_w]:
    paddle2_y -= paddle_speed
if keys[pygame.K_s]:
    paddle2_y += paddle_speed

# Update the game state
ball_x += ball_speed_x
ball_y += ball_speed_y

if ball_y &lt; 0 or ball_y &gt; screen_height - ball_radius:
    ball_speed_y *= -1

if ball_x &lt; paddle1_x + paddle_width and ball_y &gt; paddle1_y and ball_y &lt; paddle1_y + paddle_height:
    ball_speed_x *= -1
if ball_x &gt; screen_width - paddle2_x - paddle_width and ball_y &gt; paddle2_y and ball_y &lt; paddle2_y + paddle_height:
    ball_speed_x *= -1

# Draw the game
screen.fill((0, 0, 0))
pygame.draw.rect(screen, (255, 255, 255), (paddle1_x, paddle1_y, paddle_width, paddle_height))
pygame.draw.rect(screen, (255, 255, 255), (paddle2_x, paddle2_y, paddle_width, paddle_height))
pygame.draw.circle(screen, (255, 255, 255), (int(ball_x), int(ball_y)), ball_radius)

score = font.render(str(score), True, (255, 255, 255))
screen.blit(score, (screen_width / 2, 10))

pygame.display.flip()

# Cap the frame rate
pygame.time.Clock().tick(60)
</code></pre>

<p>```</p>

<p>This code creates a simple game of Pong using the Pygame library. The game has two paddles that can be controlled using the arrow keys, and a ball that bounces off the edges of the screen and the paddles. The score is displayed in the center of the screen.</p>
