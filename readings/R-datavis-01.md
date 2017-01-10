---
layout: page
element: reading
title: Data Visualization - Part 1
language: R
---

* Topics

  * `ggplot`

* Readings & videos
  * [Video introduction to ggplot](https://youtu.be/8Gew6UYqF0s) (~ 15 min)
  * [Video on transformations and statistics](https://youtu.be/jtaIvtvlGIQ) (~11 min)
  * [Video on faceting and themes](https://youtu.be/DB0kVWnk724) (~12 min)
  * [Reading for the lesson](http://swcarpentry.github.io/r-novice-gapminder/08-plot-ggplot2/) (~60 min learning + ~20 min exercises)

  * There is an error in the video -- the code for changing the legend name is incorrect. The correct code for making the plot is below and in the reading.

```r
ggplot(gapminder,
       aes(x = year, y = lifeExp)) + 
  geom_line(aes(color = continent)) + 
  facet_wrap(~country) + 
  xlab("Year") + 
  ylab("Life Expectancy") + 
  scale_colour_discrete(name="Continent") +
  theme(axis.text.x = element_blank(), 
        axis.ticks.x = element_blank())
ggsave("graphs/lifebyyearbycountry.png")
```

* Extra resources
  * [R for Data Science - Data visualisation](http://r4ds.had.co.nz/data-visualisation.html)
