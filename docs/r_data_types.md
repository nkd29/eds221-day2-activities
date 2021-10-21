---
title: "r_data_types"
author: "Nikhil D."
date: "10/21/2021"
output:  
  html_document:
    keep_md: true
---




```r
vec_1 <- c(2, 5, 9, 10, 8, 12, 1, 0)

vec_2 <- c(town = "Santa Barbara", location = "Rincon", swell = "south")

class(vec_2)
```

```
## [1] "character"
```

```r
typeof(vec_2)
```

```
## [1] "character"
```

```r
vec_2[2]
```

```
## location 
## "Rincon"
```

```r
vec_2["location"]
```

```
## location 
## "Rincon"
```

```r
vec_2_e2 <- vec_2[2]

# make dataframe
df_1 <- data.frame(region = c('A','B','A','D'),
                   species = c('otter','great white','sea lion','gray whale'),
                   count = c(12,2,36,6))
df_1
```

```
##   region     species count
## 1      A       otter    12
## 2      B great white     2
## 3      A    sea lion    36
## 4      D  gray whale     6
```

```r
# find df classes 
class(df_1)
```

```
## [1] "data.frame"
```

```r
class(df_1$species)
```

```
## [1] "character"
```

```r
max_count <- max(df_1$count)
max_count
```

```
## [1] 36
```

