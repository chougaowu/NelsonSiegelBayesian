# NelsonSiegelBayesian

I personally attach some codes in package dygraph to my packages, 
the reason is to practice how to create a package with htmlwidgets.
If there is any problem with that I will delete these parts.

This a naive analysis framework for Chinese Bonds Market, including functions for term structrue, 
notes of interesting bonds market events and possible trading strategies

Any copy of my works needs the original address attached, otherwise I hope your boom where you stand.

# Notes for 2017.5.8 to 2017.5.19
There is an interesting phenomenon in Chinese Treasury Bonds market during these two weeks,
that is the term structure seems to be downward sloping in some parts.

The problem is what cause this phenomenon, illiquidity or expectation change?

I try to model the curve and anaylze the trade records during these two weeks. The data is generated from WIND database.

# Functions of Nelson-Siegel model

Nelson and Siegel model the term structure with the following functional form, which is a whole curve modeling method

<a href="https://www.codecogs.com/eqnedit.php?latex=y_{\tau}&space;=&space;\beta_{1}&space;&plus;&space;\beta_{2}&space;\times&space;\frac{1-e^{-\tau\lambda}}{\tau\lambda}&space;&plus;&space;\beta_{3}&space;\times&space;(\frac{1-e^{-\tau\lambda}}{\tau\lambda}&space;-&space;e^{-\tau\lambda})" target="_blank"><img src="https://latex.codecogs.com/gif.latex?y_{\tau}&space;=&space;\beta_{1}&space;&plus;&space;\beta_{2}&space;\times&space;\frac{1-e^{-\tau\lambda}}{\tau\lambda}&space;&plus;&space;\beta_{3}&space;\times&space;(\frac{1-e^{-\tau\lambda}}{\tau\lambda}&space;-&space;e^{-\tau\lambda})" title="y_{\tau} = \beta_{1} + \beta_{2} \times \frac{1-e^{-\tau\lambda}}{\tau\lambda} + \beta_{3} \times (\frac{1-e^{-\tau\lambda}}{\tau\lambda} - e^{-\tau\lambda})" /></a>

Svensson extend the NS model by adding an extra term to model more complex curve structure, his function is as follows

<a href="https://www.codecogs.com/eqnedit.php?latex=y_{\tau}&space;=&space;\beta_{1}&space;&plus;&space;\beta_{2}&space;\times&space;\frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}}&space;&plus;&space;\beta_{3}&space;\times&space;(\frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}}&space;-&space;e^{-\tau\lambda_{1}})&space;&plus;&space;\beta_{4}&space;\times&space;(\frac{1-e^{-\tau\lambda_{2}}}{\tau\lambda_{2}}&space;-&space;e^{-\tau\lambda_{2}})" target="_blank"><img src="https://latex.codecogs.com/gif.latex?y_{\tau}&space;=&space;\beta_{1}&space;&plus;&space;\beta_{2}&space;\times&space;\frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}}&space;&plus;&space;\beta_{3}&space;\times&space;(\frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}}&space;-&space;e^{-\tau\lambda_{1}})&space;&plus;&space;\beta_{4}&space;\times&space;(\frac{1-e^{-\tau\lambda_{2}}}{\tau\lambda_{2}}&space;-&space;e^{-\tau\lambda_{2}})" title="y_{\tau} = \beta_{1} + \beta_{2} \times \frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}} + \beta_{3} \times (\frac{1-e^{-\tau\lambda_{1}}}{\tau\lambda_{1}} - e^{-\tau\lambda_{1}}) + \beta_{4} \times (\frac{1-e^{-\tau\lambda_{2}}}{\tau\lambda_{2}} - e^{-\tau\lambda_{2}})" /></a>



