# Boston-Housing-Dataset ( Academic Assignment )

## Problem
The Boston Housing data contain information on census tracts in Boston for which several measurements are taken (e.g., crime rate, pupil/teacher ratio). We are interested in how different variables affect the median value of owner-occupied homes in tract (represented by each row)

## Dataset

Name | Description
-----|------------
• CRIM | crime rate
• ZN | proportion of residential land zoned for lots over 25,000 sq.ft.
• INDUS | proportion of non-retail business acres per town
• CHAS | 1: if tract bounds Charles river; 0: otherwise
• NOX | nitric oxides concentration (parts per 10 million)
• RM | average number of rooms per dwelling
• AGE | proportion of owner-occupied units built prior to 1940
• DIS | weighted distances to five Boston employment centers
• RAD | index of accessibility to radial highways
• PTRATIO | pupil-teacher ratio by town
• LSTAT | Percentage of lower status of the population
• MEDV | Median value of owner-occupied homes in $1000s

## Relationship between NOX and LSTAT and MEDV
![image](https://user-images.githubusercontent.com/85646063/185258680-3e550cf4-3166-4e09-8f38-9eaca2ea374f.png)

The first conclusion that I can draw from this graph is that there is a huge number of tracts in which the nitric oxide concentration (parts per 10 million) is below 0.6 and the Percentage of lower status population is below 15. The second conclusion that can be drawn is that , overall, the median value of the occupied homes decreases with increases in LSTAT or percentage of lower status of the population and vice-versa.

## Histogram of ZN split by MEDV
![image](https://user-images.githubusercontent.com/85646063/185258961-507364bd-e66d-481c-bbb1-544273cbef18.png)

## Histogram of LSTAT split by MEDV

![image](https://user-images.githubusercontent.com/85646063/185259341-8e1f8530-4d97-48f4-937b-28447529be97.png)


LSTAT seems to be a better factor than ZN to distinguish between tracts with higher and lower median values. Although there is a slight intersection of median values greater than 20000 and median values lower than 20000 for LSTAT values between approx. 7.5 and approx. 24 , there is a huge number of tracts with median value more than 20000$ for LSTAT<15 and likewise there is a huge number of tracts with median values less than or equal to 20000$ for LSTAT>15. In the case of the ZN graph, we can see that there is a demarcation when ZN crosses 20. There seems to be more number of tracts with median values larger than 20000$ when this happens. But, the issue is that there is a huge intersection in the number of tracts with both the sets of median values (higher than 20000 and less than or equal to 20000) for 0 < ZN < 10. Hence, LSTAT seems to be a better attribute due to the low intersection value.
