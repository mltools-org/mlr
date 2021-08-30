# Multiple Linear Regression

## Import the *Marketing* dataset from the package *datarium*

*Code 1:*
```R
data("marketing", package = "datarium")
```

*Code 2:*
```R
summary(marketing)
```


*Code 2:*
```R
   youtube          facebook       newspaper          sales      
 Min.   :  0.84   Min.   : 0.00   Min.   :  0.36   Min.   : 1.92  
 1st Qu.: 89.25   1st Qu.:11.97   1st Qu.: 15.30   1st Qu.:12.45  
 Median :179.70   Median :27.48   Median : 30.90   Median :15.48  
 Mean   :176.45   Mean   :27.92   Mean   : 36.66   Mean   :16.83  
 3rd Qu.:262.59   3rd Qu.:43.83   3rd Qu.: 54.12   3rd Qu.:20.88  
 Max.   :355.68   Max.   :59.52   Max.   :136.80   Max.   :32.40  
```

```R
model <- lm(sales ~ youtube + facebook + newspaper, data = marketing)
```

```R
summary(model)
```





