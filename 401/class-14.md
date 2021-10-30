## Matplotlib 

Python package for 2D-graphics

IPython is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, it allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.

pyplot majority of plotting commands in pyplot have Matlab(TM) analogs with similar arguments. Important commands are explained with interactive examples.


### Simple plot Changing colors and line widths

![](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/exercice_3.png)

### Setting limits

![](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/exercice_4.png)


### Setting ticks
![](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/exercice_6.png)

### Subplots

With subplot you can arrange plots in a regular grid. You need to specify the number of rows and columns and the number of the plot. Note that the gridspec command is a more powerful alternative.

![](https://github.com/rougier/matplotlib-tutorial/raw/master/figures/subplot-horizontal.png)

## Animation
animation in matplotlib was not an easy task and was done mainly through clever hacks. However, things have started to change since version 1.1 and the introduction of tools for creating animation very intuitively, with the possibility to save them in all kind of formats.

most easy way to make an animation in matplotlib is to declare a FuncAnimation object that specifies to matplotlib what is the figure to update, what is the update function and what is the delay between frames.

