# Python_Day3

#Real-life use case: Calculate resistance using Ohm’s Law:
V = 10  
I = 2  
R = V / I  
print(f"The resistance is {R} ohms") 

#Mini Project
def series_circuit_check(V, R1, R2, min_current, max_current):  
    R_total = R1 + R2  
    I_total = V / R_total  
    if min_current <= I_total <= max_current:  
        return f"Current {I_total} A is within limits."  
    else:  
        return f"Current {I_total} A is NOT within limits."  
print(series_circuit_check(20, 4, 6, 1.5, 2.5))  
