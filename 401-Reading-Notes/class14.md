# 401 Class 13 Reading Notes

## Summary: This class is about Data Visualization tools Matplotlib, bokah, Seaborn 


 Q: What are the key differences between Matplotlib, Seaborn, and Bokeh libraries in terms of their features and use cases? Provide an example of a specific visualization that is more suitable for each library.

A: Matplotlib, Seaborn, and Bokeh are popular data visualization libraries in Python, and each has its own strengths and use cases.

Matplotlib is a versatile library that can create a wide range of static visualizations, including line charts, scatter plots, bar charts, histograms, and more. It is a powerful library that allows for a high degree of customization, but can require more code to create complex plots.

An example of a visualization that is well-suited for Matplotlib would be a time series line chart showing the stock price of a company over a period of time. This is because Matplotlib has a lot of flexibility in terms of customization and can handle the complexity of the visualization.

Seaborn, on the other hand, is a library that is built on top of Matplotlib and provides a higher-level interface for creating statistical visualizations. Seaborn is particularly well-suited for creating visualizations that display relationships between variables, such as scatter plots with regression lines or heatmaps. It also provides a set of default themes that make it easy to create attractive plots with minimal customization.

An example of a visualization that is well-suited for Seaborn would be a scatter plot with a regression line showing the relationship between a person's age and their income. Seaborn's built-in regression plot function can make it easy to create this type of visualization with just a few lines of code.

Bokeh is a library that is designed for creating interactive visualizations for the web. It allows for the creation of complex, interactive plots that can be embedded in web pages or Jupyter notebooks. Bokeh is particularly well-suited for visualizations that require user interaction, such as zooming or panning.

An example of a visualization that is well-suited for Bokeh would be a geographic map that allows users to zoom in and out and view different layers of data, such as population density or weather patterns. Bokeh's interactive tools and support for web technologies make it an ideal choice for this type of visualization.



Q: In the Seaborn library, what are the main functions to create relational, categorical, and distribution plots? Briefly explain the purpose of each type of plot and provide an example use case.

A: Seaborn is a popular Python library for creating statistical visualizations. It provides a number of functions for creating different types of plots, including relational, categorical, and distribution plots.

Relational plots:
Relational plots are used to show the relationship between two variables. Seaborn provides a number of functions for creating relational plots, including scatter plots, line plots, and joint plots.

An example use case for a scatter plot would be to visualize the relationship between a person's height and weight. The scatterplot function in Seaborn can be used to create this type of visualization.

Categorical plots:
Categorical plots are used to show the relationship between a numerical variable and a categorical variable. Seaborn provides a number of functions for creating categorical plots, including box plots, violin plots, and swarm plots.

An example use case for a box plot would be to visualize the distribution of test scores for different groups of students. The boxplot function in Seaborn can be used to create this type of visualization.

Distribution plots:
Distribution plots are used to show the distribution of a numerical variable. Seaborn provides a number of functions for creating distribution plots, including histograms, kernel density plots, and rug plots.

An example use case for a kernel density plot would be to visualize the distribution of salaries for a group of employees. The kdeplot function in Seaborn can be used to create this type of visualization.

In summary, Seaborn provides a variety of functions for creating different types of plots, each with their own specific purpose. Relational plots show the relationship between two variables, categorical plots show the relationship between a numerical variable and a categorical variable, and distribution plots show the distribution of a numerical variable.



Q: Discuss the role of the Seaborn Cheat Sheet in a Python developer’s workflow. What are some key sections or elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities?

A: The Seaborn Cheat Sheet is a quick reference guide that summarizes the main features and functionalities of the Seaborn library. It is a valuable tool for Python developers who are using Seaborn for data visualization and want to quickly reference the different functions and options available to them.

The cheat sheet is divided into several sections, each of which covers a different aspect of the Seaborn library. Some key sections and elements featured in the cheat sheet that can help a developer quickly reference Seaborn functionalities include:

Importing Seaborn: This section covers the basic syntax for importing Seaborn into a Python script.

Dataset loading: This section covers the functions for loading built-in datasets provided by Seaborn, such as tips, iris, and titanic.

Figure aesthetics: This section covers the options for customizing the appearance of Seaborn plots, such as changing the color palette, adding grid lines, and modifying axis labels.

Relational plots: This section covers the functions for creating different types of relational plots, such as scatter plots, line plots, and joint plots. It also covers options for customizing the appearance of these plots, such as changing the point size and marker style.

Categorical plots: This section covers the functions for creating different types of categorical plots, such as box plots, violin plots, and swarm plots. It also covers options for customizing the appearance of these plots, such as changing the box width and orientation.

Distribution plots: This section covers the functions for creating different types of distribution plots, such as histograms, kernel density plots, and rug plots. It also covers options for customizing the appearance of these plots, such as changing the bin size and bandwidth.

Overall, the Seaborn Cheat Sheet can be a valuable tool for Python developers who are using Seaborn for data visualization. It provides a quick reference guide to the main features and functionalities of the library, making it easier for developers to create effective and visually appealing visualizations.


### What is Bokeh?

Bokeh is an interactive visualization library that targets modern web browsers for presentation. It is good for:

Interactive visualization in modern browsers
Standalone HTML documents, or server-backed apps
Expressive and versatile graphics
Large, dynamic or streaming data
Easy usage from python (or Scala, or R, or...)
And most importantly:


## Sources: 
ChatGPT

https://hub.gke2.mybinder.org/user/bokeh-bokeh-notebooks-w24rwohe/notebooks/tutorial/00%20-%20Introduction%20and%20Setup.ipynb

https://seaborn.pydata.org/tutorial.html

https://github.com/rougier/matplotlib-tutorial

 ## Things I want to know more about
 
 Time Series Data




