# Statistical terms

<br>

## **Content**
- [Coefficient of Determination (R-squared)](#coefficient-of-determination-r-squared)
- [Coefficient of Variation (CV)](#coefficient-of-variation-cv)
- [Correlation Coefficient (Pearson's r)](#correlation-coefficient-pearsons-r)
- [Covariance](#covariance)
- [Mean](#mean)
- [Standard Deviation](#standard-deviation)
- [Variance](#variance)

<br>

## **Coefficient of Determination (R-squared)**
- The **coefficient of determination** is a measure of how well the regression line represents the data.
$$ R^2 = 1 - \frac{SS_{res}}{SS_{tot}} $$
$$ SS_{res} = \sum_{i=1}^{n} (y_i - \hat{y}_i)^2 $$
$$ SS_{tot} = \sum_{i=1}^{n} (y_i - \bar{y})^2 $$
- Where
    - $ n $ is the number of data points
    - $ y_i $ is the $ i^{th} $ data point of the dependent variable
    - $ \hat{y}_i $ is the $ i^{th} $ predicted value of the dependent variable
    - $ \bar{y} $ is the [mean](#mean) of the dependent variable
    - $ SS_{res} $ is the sum of squares of residuals
    - $ SS_{tot} $ is the total sum of squares
- **HINT**: In linear least squares multiple regression (with fitted intercept and slope), $R^2$ equals $\rho^2(y, \hat{y})$, the square of the [Pearson correlation coefficient](#correlation-coefficient-pearsons-r-pcc) between the observed $y$ and modeled (predicted) $\hat{y}$ data values of the dependent variable.

<br>

## **Coefficient of Variation (CV)**
- In probability theory and statistics, the **coefficient of variation (CV)**, also known as normalized root-mean-square deviation (NRMSD), **percent RMS**, and **relative standard deviation (RSD)**, is a standardized measure of dispersion of a probability distribution or frequency distribution. 
- It is defined as the ratio of the standard deviation $\sigma$ to the mean $\mu$ (or its absolute value, $|\mu|$), and often expresses as a percentage (%RSD).
- The CV or RSD is widely used in analytical chemistry to express the precision and repeatability of an assay.
- For Percent CV, multiply the coefficient of variation by 100.
### For Population
$$ CV = \frac{\sigma}{\mu}$$
- Where
    - $ \sigma $ is the [standard deviation](#standard-deviation) of the population
    - $ \mu $ is the [mean](#mean) of the population

### For Sample
$$ CV = \frac{s}{\bar{x}}$$
- Where
    - $ s $ is the [standard deviation](#standard-deviation) of the sample
    - $ \bar{x} $ is the [mean](#mean) of the sample

<br>

## **Correlation Coefficient (Pearson's r)**
| Correlation Coefficient | Strength of Relationship | Correlation Type |
| --- | --- | --- |
|-.7 to -1 | Very string | Negative |
|-.5 to -.7 | Strong | Negative |
|-.3 to -.5 | Moderate | Negative |
|-.1 to -.3 | Weak | Negative |
|0 | None | Zero |
|.1 to .3 | Weak | Positive |
|.3 to .5 | Moderate | Positive |
|.5 to .7 | Strong | Positive |
|.7 to 1 | Very strong | Positive |
- The Pearson’s product-moment correlation coefficient, also known as Pearson’s r, describes the linear relationship between two quantitative variables.

### For Population
$$ \rho_{X, Y} = \frac{Cov(X, Y)}{\sigma_X \sigma_Y} $$
- Where
    - $ Cov(X, Y) $ is the [covariance](#covariance) between $ X $ and $ Y $
    - $ \sigma_X $ is the [standard deviation](#standard-deviation) of $ X $
    - $ \sigma_Y $ is the [standard deviation](#standard-deviation) of $ Y $

<br>

### For Sample
$$ r_{x, y} = \frac{Cov(x, y)}{s_x s_y} $$
- Where
    - $ Cov(x, y) $ is the [covariance](#covariance) between $ x $ and $ y $
    - $ s_x $ is the [standard deviation](#standard-deviation) of $ x $
    - $ s_y $ is the [standard deviation](#standard-deviation) of $ y $

<br>

## **Covariance**
- In probability theory and statistics, **covariance** is a measure of the joint variability of two random variables.
- The sign of the covariance, therefore, shows the tendency in the linear relationship between the variables
    - **Positive**: the variables tend to increase together
    - **Negative**: one variable tends to decrease as the other increases
    - **Zero**: the variables are independent
- The [correlation coefficient](#correlation-coefficient-pearsons-r-pcc) normalizes the covariance by dividing by the geometric mean of the total variances for the two random variables.
- The Covariance of the same variable is the variance of that variable.

### For Population
$$ Cov(X, Y) = \frac{1}{n} \sum_{i=1}^{n} (X_i - \hat{X})(Y_i - \hat{Y}) $$
$$ Cov(X, X) = \sigma^2 $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point of $ X $
    - $ \hat{X} $ is the [mean](#mean) of $ X $
    - $ Y_i $ is the $ i^{th} $ data point of $ Y $
    - $ \hat{Y} $ is the [mean](#mean) of $ Y $

<br>

### For Sample
$$ Cov(X, Y) = \frac{1}{n - 1} \sum_{i=1}^{n} (X_i - \bar{X})(Y_i - \bar{Y}) $$
$$ Cov(X, X) = s^2 $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point of $ X $
    - $ \bar{X} $ is the [mean](#mean) of $ X $
    - $ Y_i $ is the $ i^{th} $ data point of $ Y $
    - $ \bar{Y} $ is the [mean](#mean) of $ Y $

<br>

## **Mean**
- The **mean** is the average of the data points
$$ \bar{X} = \mu = \frac{1}{n} \sum_{i=1}^{n} X_i $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point

<br>

## **Standard Deviation**

### For Population
$$ \sigma = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (X_i - \mu)^2} $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point
    - $ \mu $ is the [mean](#mean) of the data points

### For Sample
$$ s = \sqrt{\frac{1}{n - 1} \sum_{i=1}^{n} (X_i - \bar{X})^2} $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point
    - $ \bar{X} $ is the [mean](#mean) of the data points

<br>

## **Variance**

### For Population
$$ \sigma^2 = \frac{1}{n} \sum_{i=1}^{n} (X_i - \mu)^2 $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point
    - $ \mu $ is the [mean](#mean) of the data points

<br>

### For Sample
$$ s^2 = \frac{1}{n - 1} \sum_{i=1}^{n} (X_i - \bar{X})^2 $$
- Where
    - $ n $ is the number of data points
    - $ X_i $ is the $ i^{th} $ data point
    - $ \bar{X} $ is the [mean](#mean) of the data points