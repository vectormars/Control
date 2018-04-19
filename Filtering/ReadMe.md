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









________________________________________________________________________________________________________________________

Based on: [Kalman-and-Bayesian-Filters-in-Python](https://github.com/vectormars/Kalman-and-Bayesian-Filters-in-Python)
