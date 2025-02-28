# Conwoy game of life

# What is Conway's Game of Life?
Conway's Game of Life is a cellular automaton that is played on a 2D square grid. Each square (or "cell") on the grid can be either alive or dead, and they evolve according to the following rules:
<br>
Any live cell with fewer than two live neighbours dies (referred to as underpopulation).<br>
Any live cell with more than three live neighbours dies (referred to as overpopulation).<br>
Any live cell with two or three live neighbours lives, unchanged, to the next generation.<br>
Any dead cell with exactly three live neighbours comes to life.

# How do we created this game ?
<br>
we used to build this game a javascript code
<br>
so the most important thing is usage of object orient programming
<br>
and so applying its pillars made the code very clear and goergous to understand

# Code

so firstly we created a simple html page and applied a fewer styles.
<br>
and secondly we started to code the javascript
<br>
So in javascript we created two classes that are very usefull to improve the
functionnality
here is diagram class

                            ------------------------
                                    Game     
                            ------------------------
                                rows
                                cols
                                cellSize
                                grid
                                isRunning
                            ------------------------
                            Game(rows, cols, cellSize)
                                createEmptyGrid()
                                randomize()
                                drawGliderGun()
                                drawPulsar()
                                drawPentaDecathlon()
                                countNeighbors(x, y)
                                update()
                            --------------------------


                            --------------------------
                                    Renderer
                            --------------------------
                                    canvas
                                    ctx
                                    game
                            ------------------------
                            Render(canvas, game)
                            draw()
                            --------------------------


# understanding every method
<br>
- for Game Class
the constructor initialize all the attribute declared
<br>
createEmptyGrid() creates an empty grid without any full cell
<br>
randomize() brings alive some random cells
<br>
drawGliderGun() draws a glider gun by made some cells alive as the draw
<br>
drawPulsar() the same function as the other it draw a pulsar draw
<br>
drawPentaDecathlon() the same idea but its penta decathlon
<br>
countNeigbours(x, y) counts the alive cells between a given cell
<br>
update() starts the action of evolving those cells
<br>
- for Renderer Class
the constructor initialize all the attribute declared
<br>
draw() initialize the canva
<br>
that's all for the classes
<br>
in order to perform we used some event listeners in many DOM elements
<br>
espicially the button and document
<br>
for the main event of listner and which is the DOMContentLoaded and that
<br>
called after all the html tags loaded and styles are applied
<br>
and for that it starts by a callback that do these steps:
instanciate all the classes that we created
<br>
After that the click event for startBtn and for that it changes the status
of the game from stop to start
<br>
and then update the game and draw 
<br>
After this we have clearBtn 
<br>
by calling game.createEmptyGrid() and then draw

After that random button<br>
call game.random() and draw()<br>

and for gilder gun and pulsar and pentadecathlon events<br>

call every game.gilderGun() or .pulsar() or .pentadecathlon()<br>

and then draw() <br>

and that's all for the functionnalities for this game and Thanks :)
