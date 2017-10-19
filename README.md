## Spatial SIR model of a zombie outbreak in France

This simple SIR model simulates a zombie outbreak in France, inspired by the scenario described in [When zombies attack!: Mathematical modeling of an outbreak of zombie infection](http://loe.org/images/content/091023/Zombie%20Publication.pdf).

Here the model is extended spatially to allow neighboring grid cells to interact with one another (each cell can interact with its 8 adjacent cells) so infection can spread from cell to cell, and the global zombie outbreak can be visually appreciated (who doesn't want to see a nice zombie wave!).

The patient zero (there must be one ...) is placed somewhere between Lyon and Nimes.

The two line charts on the right show the current state of the population for each iteration of the model:

- Red: zombie wave (on the map) and percentage of living population that is infected (top line chart)
- Blue: living people (on the map) and remaining percentage of living population (bottom line chart)
- Green: dead people (on the map) and percentage of living population that died from the zombie outbreak (bottom line chart)

The France population density image is created from the published [2011 Europe Population grid data](http://ec.europa.eu/eurostat/web/gisco/geodata/reference-data/population-distribution-demography) (see the `formatData` function in this [file](https://github.com/gcalmettes/spatial-SIR/blob/master/js/zombie.js) for the details of how the data are transformed to the grid format).