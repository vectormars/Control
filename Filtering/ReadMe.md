## Key points
* Multiple data points are more accurate than one data point, so throw nothing away no matter how inaccurate it is.
* Always choose a number part way between two data points to create a more accurate estimate.
* Predict the next measurement and rate of change based on the current estimate and how much we think it will change.
* The new estimate is then chosen as part way between the prediction and next measurement scaled by how accurate each is.

________________________________________________________________________________________________________________________

### g-h filter
1. [g-h filter introduction](Code/G-H%20filter%20introduction.ipynb)  
2. [g-h filter](Code/G-H%20filter.ipynb)
3. [g-h filter Train example](Code/G-H%20filter%20Train%20example.ipynb)

Notes:
1. Our model assumes that velocity is constant. Not able to follow the effect of acceleration.
2. Larger ```g``` we more closely follow the measurement instead of the prediction.
3. We not only filter out noise, but legitimate changes in the signal as well. Larger ```g``` follow the state change more closely.
4. If our signal is changing a lot (quickly relative to the time step of our filter), then a large ```h``` will cause us to react to those transient changes rapidly.

________________________________________________________________________________________________________________________

### Discrete Bayes Filter
The Kalman filter belongs to a family of filters called Bayesian filters.
1. [Introduction](Code/Discrete%20Bayes%20Filter-Intro.ipynb)
2. [Algorithm](Code/Discrete%20Bayes%20Algorithm.ipynb)

### One Dimensional Kalman Filters
1. [1D Gaussians](Code/Gaussians.ipynb)
2. [Bayes Theorem](Code/Bayes%20Theorem.ipynb)
3. [Introduction](Code/One-Dimensional-Kalman-Filters-Intro.ipynb)
4. [Algorithm](Code/One-Dimensional-Kalman-Filters.ipynb)

### Multivariate Kalman Filters
1. [Correlation and Covariance](Code/Multivariate%20Gaussians-Correlation%20and%20Covariance.ipynb)
2. [Multivariate Normal Distribution Equation](Code/Multivariate%20Gaussians-Equations.ipynb)
3. [Multiplying Multidimensional Gaussians](Code/Multivariate%20Gaussians-Multiplying.ipynb)
4. [Hidden Variables](Code/Multivariate%20Gaussians-Hidden%20Variables.ipynb)
5. [Introduction](Code/Multivariate%20Kalman%20Filters-Introduction.ipynb)
6. [Algorithm](Code/Multivariate%20Kalman%20Filters-Equations.ipynb)


### Smoothing
1. [Introduction](Code/Smoothing.ipynb)
2. [Fixed-Interval Smoothing](Code/Smoothing_Fixed_Interval.ipynb)
3. [Fixed-Lag Smoothing](Code/Smoothing_Fixed_Lag.ipynb)
4. Fixed-Point Smoothing

### Adaptive filtering
1. [Introduction](Code/Adaptive%20Filtering%20-%20Introduction.ipynb)      
2. [Detecting a Maneuver](Code/Adaptive%20Filtering-Detecting%20a%20Maneuver.ipynb)

### Robust Kalman
[Robust Kalman](Code/Robust%20Kalman.ipynb)
________________________________________________________________________________________________________________________

Based on:        
[Kalman-and-Bayesian-Filters-in-Python](https://github.com/rlabbe/Kalman-and-Bayesian-Filters-in-Python)          
[Robust Kalman](https://github.com/milsto/robust-kalman)
