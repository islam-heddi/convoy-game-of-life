# Convoy game of life

# What is Conway's Game of Life?
Conway's Game of Life is a cellular automaton that is played on a 2D square grid. Each square (or "cell") on the grid can be either alive or dead, and they evolve according to the following rules:

Any live cell with fewer than two live neighbours dies (referred to as underpopulation).
Any live cell with more than three live neighbours dies (referred to as overpopulation).
Any live cell with two or three live neighbours lives, unchanged, to the next generation.
Any dead cell with exactly three live neighbours comes to life.

# How do we created this game ?

we used to build this game a javascript code

so the most important thing is usage of object orient programming

and so applying its pillars made the code very clear and goergous to understand

# Code

so firstly we created a simple html page and applied a fewer styles.

and secondly we started to code the javascript

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