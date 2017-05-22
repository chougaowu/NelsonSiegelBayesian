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

Svensson extend the NS model by adding an extra term to model more complex
