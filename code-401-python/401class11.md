# # class 11
## Data Visualization

Matplotlib comes with a set of default settings that allow customizing all kinds of properties. You can control the defaults of almost every property in matplotlib: figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on

A figure in matplotlib means the whole window in the user interface. Within this figure there can be subplots. While subplot positions the plots in a regular grid, axes allows free placement within the figure.

When we call plot, matplotlib calls gca() to get the current axes and gca in turn calls gcf() to get the current figure. If there is none it calls figure() to make one, strictly speaking, to make a subplot(111). Let's look at the details.

With subplot you can arrange plots in a regular grid. You need to specify the number of rows and columns and the number of the plot.

The most easy way to make an animation in matplotlib is to declare a FuncAnimation object that specifies to matplotlib what is the figure to update, what is the update function and what is the delay between frames.


What is Bokeh¶ Bokeh is an interactive visualization library that targets modern web browsers for presentation. It is good for:

Interactive visualization in modern browsers Standalone HTML documents, or server-backed apps Expressive and versatile graphics Large, dynamic or streaming data Easy usage from python (or Scala, or R, or...) And most importantly:

NO JAVASCRIPT REQUIRED Bokeh is an interactive visualization library for modern web browsers. It provides elegant, concise construction of versatile graphics, and affords high-performance interactivity over large or streaming datasets. Bokeh can help anyone who would like to quickly and easily make interactive plots, dashboards, and data applications.