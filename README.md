# Temporal_Logic_Point_Processes
codes of paper "Temporal Logic Point Processes", ICML 2020

Synthetic data demo:

function: "generate_synthetic_data.py" -- it is used to generated synthetic event data given prespecified rules

function: " logic_template.py" --- it is used to learn model parameters given the prespecified logic templates and the input event data.

Logic templates introduced here look like: 

# for example, consider three rules:

    # A and B and Equal(A,B), and Before(A, D), then D;
    
    # C and Before(C, Not D), then  Not D
    
    # D Then  E, and Equal(D, E)
