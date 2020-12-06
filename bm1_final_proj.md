BM1 final project
================

    ## 'data.frame':    51 obs. of  9 variables:
    ##  $ state                                  : chr  "Alabama" "Alaska" "Arizona" "Arkansas" ...
    ##  $ unemployment                           : chr  "high" "high" "high" "high" ...
    ##  $ urbanization                           : chr  "low" "low" "high" "low" ...
    ##  $ median_household_income                : int  42278 67629 49254 44922 60487 60940 70161 57522 68277 46140 ...
    ##  $ perc_population_with_high_school_degree: num  0.821 0.914 0.842 0.824 0.806 0.893 0.886 0.874 0.871 0.853 ...
    ##  $ perc_non_citizen                       : num  0.02 0.04 0.1 0.04 0.13 0.06 0.06 0.05 0.11 0.09 ...
    ##  $ gini_index                             : num  0.472 0.422 0.455 0.458 0.471 0.457 0.486 0.44 0.532 0.474 ...
    ##  $ perc_non_white                         : num  0.35 0.42 0.49 0.26 0.61 0.31 0.3 0.37 0.63 0.46 ...
    ##  $ hate_crimes_per_100k_splc              : chr  "0.125838926" "0.143740118" "0.225319954" "0.069060773" ...

    ## 'data.frame':    51 obs. of  9 variables:
    ##  $ state                                  : chr  "Alabama" "Alaska" "Arizona" "Arkansas" ...
    ##  $ unemployment                           : Factor w/ 2 levels "high","low": 1 1 1 1 1 2 1 2 1 1 ...
    ##  $ urbanization                           : Factor w/ 2 levels "high","low": 2 2 1 2 1 1 1 1 1 1 ...
    ##  $ median_household_income                : int  42278 67629 49254 44922 60487 60940 70161 57522 68277 46140 ...
    ##  $ perc_population_with_high_school_degree: num  0.821 0.914 0.842 0.824 0.806 0.893 0.886 0.874 0.871 0.853 ...
    ##  $ perc_non_citizen                       : num  0.02 0.04 0.1 0.04 0.13 0.06 0.06 0.05 0.11 0.09 ...
    ##  $ gini_index                             : num  0.472 0.422 0.455 0.458 0.471 0.457 0.486 0.44 0.532 0.474 ...
    ##  $ perc_non_white                         : num  0.35 0.42 0.49 0.26 0.61 0.31 0.3 0.37 0.63 0.46 ...
    ##  $ hate_crimes_per_100k_splc              : num  0.1258 0.1437 0.2253 0.0691 0.2558 ...

## Descriptive statistics+Graphs

    ## 
    ## Table: Descriptive Characteristics of Study Sample, Hate Crimes Occurring in the United States (By State)
    ## 
    ## |                                                         |   Overall (N=51)    |
    ## |:--------------------------------------------------------|:-------------------:|
    ## |Hate crime rate per 100k population                      |                     |
    ## |-  Mean/SD                                               |     0.30 (0.25)     |
    ## |-  Median                                                |        0.23         |
    ## |-  IQR                                                   |        0.21         |
    ## |-  Min - Max                                             |     0.07 - 1.52     |
    ## |-  Missing                                               |          4          |
    ## |Level of state unemployment                              |                     |
    ## |-  high                                                  |     24 (47.1%)      |
    ## |-  low                                                   |     27 (52.9%)      |
    ## |-  Missing                                               |          0          |
    ## |Level of state urbanization                              |                     |
    ## |-  high                                                  |     24 (47.1%)      |
    ## |-  low                                                   |     27 (52.9%)      |
    ## |-  Missing                                               |          0          |
    ## |Median household income per state                        |                     |
    ## |-  Mean/SD                                               | 55223.61 (9208.48)  |
    ## |-  Median                                                |      54916.00       |
    ## |-  IQR                                                   |      12062.00       |
    ## |-  Min - Max                                             | 35521.00 - 76165.00 |
    ## |-  Missing                                               |          0          |
    ## |Percentage of adults (>25 yrs) with a high school degree |                     |
    ## |-  Mean/SD                                               |     0.87 (0.03)     |
    ## |-  Median                                                |        0.87         |
    ## |-  IQR                                                   |        0.06         |
    ## |-  Min - Max                                             |     0.80 - 0.92     |
    ## |-  Missing                                               |          0          |
    ## |Percentage of population that are not US citizens        |                     |
    ## |-  Mean/SD                                               |     0.05 (0.03)     |
    ## |-  Median                                                |        0.04         |
    ## |-  IQR                                                   |        0.05         |
    ## |-  Min - Max                                             |     0.01 - 0.13     |
    ## |-  Missing                                               |          3          |
    ## |Gini index                                               |                     |
    ## |-  Mean/SD                                               |     0.45 (0.02)     |
    ## |-  Median                                                |        0.45         |
    ## |-  IQR                                                   |        0.03         |
    ## |-  Min - Max                                             |     0.42 - 0.53     |
    ## |-  Missing                                               |          0          |
    ## |Percentage of population that are non-white              |                     |
    ## |-  Mean/SD                                               |     0.32 (0.16)     |
    ## |-  Median                                                |        0.28         |
    ## |-  IQR                                                   |        0.22         |
    ## |-  Min - Max                                             |     0.06 - 0.81     |
    ## |-  Missing                                               |          0          |

<img src="bm1_final_proj_files/figure-gfm/unnamed-chunk-2-1.png" width="90%" />

## Varible Selection

<img src="bm1_final_proj_files/figure-gfm/unnamed-chunk-3-1.png" width="90%" />

    ##                                         median_household_income
    ## median_household_income                                    1.00
    ## perc_population_with_high_school_degree                    0.65
    ## perc_non_citizen                                           0.30
    ## gini_index                                                -0.13
    ## perc_non_white                                             0.04
    ## hate_crimes_per_100k_splc                                  0.34
    ##                                         perc_population_with_high_school_degree
    ## median_household_income                                                    0.65
    ## perc_population_with_high_school_degree                                    1.00
    ## perc_non_citizen                                                          -0.26
    ## gini_index                                                                -0.54
    ## perc_non_white                                                            -0.50
    ## hate_crimes_per_100k_splc                                                  0.26
    ##                                         perc_non_citizen gini_index
    ## median_household_income                             0.30      -0.13
    ## perc_population_with_high_school_degree            -0.26      -0.54
    ## perc_non_citizen                                    1.00       0.48
    ## gini_index                                          0.48       1.00
    ## perc_non_white                                      0.75       0.55
    ## hate_crimes_per_100k_splc                           0.24       0.38
    ##                                         perc_non_white
    ## median_household_income                           0.04
    ## perc_population_with_high_school_degree          -0.50
    ## perc_non_citizen                                  0.75
    ## gini_index                                        0.55
    ## perc_non_white                                    1.00
    ## hate_crimes_per_100k_splc                         0.11
    ##                                         hate_crimes_per_100k_splc
    ## median_household_income                                      0.34
    ## perc_population_with_high_school_degree                      0.26
    ## perc_non_citizen                                             0.24
    ## gini_index                                                   0.38
    ## perc_non_white                                               0.11
    ## hate_crimes_per_100k_splc                                    1.00

## Model building

``` r
# Varibale Selection- Stepwise
res1 <- lm(hate_crimes_per_100k_splc ~ unemployment + urbanization + 
             median_household_income + perc_population_with_high_school_degree +
             perc_non_citizen + gini_index + perc_non_citizen , data=crimes)

summary(res1)
```

    ## 
    ## Call:
    ## lm(formula = hate_crimes_per_100k_splc ~ unemployment + urbanization + 
    ##     median_household_income + perc_population_with_high_school_degree + 
    ##     perc_non_citizen + gini_index + perc_non_citizen, data = crimes)
    ## 
    ## Residuals:
    ##      Min       1Q   Median       3Q      Max 
    ## -0.36516 -0.10256 -0.01341  0.09717  0.51338 
    ## 
    ## Coefficients:
    ##                                           Estimate Std. Error t value Pr(>|t|)
    ## (Intercept)                             -8.303e+00  1.831e+00  -4.535 5.62e-05
    ## unemploymentlow                          1.334e-02  6.879e-02   0.194  0.84729
    ## urbanizationlow                          3.301e-02  8.349e-02   0.395  0.69478
    ## median_household_income                 -1.518e-06  5.818e-06  -0.261  0.79558
    ## perc_population_with_high_school_degree  5.391e+00  1.721e+00   3.133  0.00333
    ## perc_non_citizen                         1.217e+00  1.554e+00   0.783  0.43846
    ## gini_index                               8.621e+00  1.941e+00   4.441 7.48e-05
    ##                                            
    ## (Intercept)                             ***
    ## unemploymentlow                            
    ## urbanizationlow                            
    ## median_household_income                    
    ## perc_population_with_high_school_degree ** 
    ## perc_non_citizen                           
    ## gini_index                              ***
    ## ---
    ## Signif. codes:  0 '***' 0.001 '**' 0.01 '*' 0.05 '.' 0.1 ' ' 1
    ## 
    ## Residual standard error: 0.1987 on 38 degrees of freedom
    ##   (6 observations deleted due to missingness)
    ## Multiple R-squared:  0.461,  Adjusted R-squared:  0.3759 
    ## F-statistic: 5.417 on 6 and 38 DF,  p-value: 0.0003982
