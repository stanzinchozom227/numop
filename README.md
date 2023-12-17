import numpy as np
from scipy.optimize import minimize_scalar
def objective_function(x):
return -(x**2 + 2*x + 1)
print()
min_result = minimize_scalar(objective_function, method='golden', bracket=(0, 1))
max_result = minimize_scalar(objective_function, method='golden', bracket=(0, 1))
optimal_max_solution = max_result.x 
optimal_min_solution = min_result.x
print("Maximization Result - Optimal Solution :", optimal_max_solution)
print("Minimization Result - Optimal Solution :", optimal_min_solution)

output:
maximization result: optimal solution:1.34078079514178e+154
minimization result: optimal solution:1.34078079514178e+154
