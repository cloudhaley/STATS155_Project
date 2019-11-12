---
title: "data_explore"
output: 
  html_document:
    keep_md: yes

---

Drop your plots below :)


```r
library(fivethirtyeight)
library(ggplot2)
```


```r
ggplot(data = hiphop_cand_lyrics)+
  geom_boxplot(aes(x = candidate, y = album_release_date))
```

![](data_explore_files/figure-html/unnamed-chunk-2-1.png)<!-- -->
