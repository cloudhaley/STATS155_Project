---
title: "data_explore"
author: "Haley Vien, Maria Aerrola, Tara Mercene, Cathlyn Liang"
output: 
  html_document:
    keep_md: yes
    df_print: paged

---

Drop your plots below :)



```r
library(fivethirtyeight)
library(ggplot2)
data("bachelorette")
library(broom)
library(moderndive)
library(tidyverse)
library(openintro)
```

Maria's graph

```r
ggplot(data = hiphop_cand_lyrics)+
  geom_boxplot(aes(x = candidate, y = album_release_date))
```

![](data_explore_files/figure-html/unnamed-chunk-2-1.png)<!-- -->


Haley's graph


```r
hiphop_cand_lyrics %>% 
  ggplot() +
  geom_jitter(aes(x=sentiment, y=candidate, color = candidate))
```

![](data_explore_files/figure-html/unnamed-chunk-3-1.png)<!-- -->




```r
ggplot(data = bachelorette)+
  geom_boxplot(aes(x = show, y = season, fill = show))
```

![](data_explore_files/figure-html/unnamed-chunk-4-1.png)<!-- -->


```r
ggplot(data = bachelorette)+
  geom_histogram(aes(x = season), bins = 50)
```

![](data_explore_files/figure-html/unnamed-chunk-5-1.png)<!-- -->





