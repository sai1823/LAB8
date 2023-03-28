# LAB8
LAB 8 Interactive Graph with Shiny

This is a Shiny app that creates a scatter plot of the iris dataset. 
The app allows the user to select the variables to plot on the x-axis and y-axis, as well as the color, shape, and size of the points. 
The user can also select the species of iris to highlight in a different color and shape.

The app uses the read.csv function from the utils package to read in the iris dataset from a URL. 
The UI is created using the fluidPage function from the shiny package. 
It includes a title panel, a header, a paragraph, a sidebar layout, and a main panel. 
The sidebar panel includes several input controls such as select inputs for x-axis variable, y-axis variable, color, shape, and species. 
It also includes a slider input for point size. 
The main panel includes a plot output for the scatter plot.

The server function defines the reactive behavior of the app. 
It uses the renderPlot function to render the scatter plot based on the user's input selections. 
The x-axis variable and y-axis variable are extracted from the iris_data data frame based on the user's input. 
The colors of the points are determined by the user's selection of colors for the two species. 
The shapes of the points are determined by the user's selection of shape for the highlighted species. 
The scatter plot is then created using the ggplot function from the ggplot2 package, and various aesthetics such as color, shape, and size are defined. 
Finally, the plot is output to the scatterPlot output element in the UI.

