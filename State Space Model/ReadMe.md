### Solve Differential Equations in Python
Differential equations are solved in Python with the Scipy.integrate package using function ODEINT. ODEINT requires three inputs:      
```
 y = odeint(model, y0, t)
```
1. **model**: Function name that returns derivative values at requested y and t values as dydt = model(y,t)
2. **y0**: Initial conditions of the differential states
3. **t**: Time points at which the solution should be reported. Additional internal points are often calculated to maintain accuracy of the solution but are not reported.

[Eg](Code/ODEINT.ipynb)
