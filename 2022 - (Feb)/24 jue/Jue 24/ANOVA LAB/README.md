## <p align="center"> FOR THE DATA USED IN JUPYTER NOTEBOOK :mag: </p>
| QUESTION | ANSWER |
|---|---|
| **Null hypothesis** | There is no relationship between the power and the etching. |
| **Alternate hypothesis** | There is a relationship between the power and the etching. |
| **Level of significance** | If the p level is under 0,05, we can say with a 95% confidence that the alternate hypothesis is true. /n In this case, it is, so we can refuse the null hypothesis. |
| **Degrees of freedom** | We have three unique power readings, so the degrees of freedom are this number minus one (in this case, two). |
| **Error terms** | Errors or residuals are the segments of scores not accounted for by the analysis. |
| **Total degrees of freedom** | We have 20 observations, so the total DoF is 19 (total readings minus one), as we are looking at sample averages. |

***

### Now, what do the results tell us?

|| df | sum_sq	| mean_sq |	F |	PR(>F)|
|---|---|---|---|---|---|
| C(power) |	2.0	| 18.176653	| 9.088327	| 36.878955	| 0.000008 |
| Residual	| 12.0	| 2.957240	| 0.246437	| NaN	| NaN |

### What about the means?

|**MEANS**||
|---|---|
| 160 W | 5.792000 |
| 180 W | 6.238000 |
| 200 W | 8.318000 |

![means barchart](https://github.com/JosepTrota/Main-Workspace/blob/main/Feb%2022/Jue%2024/ANOVA%20LAB/Barchart%20average%20etching.png?raw=true)

***

## **CONCLUSIONS**

According to thedata given, there clearly seems to be a relationship between the power and the etching, so to make business decisions taking that into account would be wise.
If you want more etching, you have to use more power :muscle:

***
