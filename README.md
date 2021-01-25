# Temporal_Logic_Point_Processes
codes of paper "Temporal Logic Point Processes", ICML 2020

Synthetic data demo:

function: "generate_synthetic_data.py" -- it is used to generated synthetic event data given prespecified rules

function: " logic_template.py" --- it is used to learn model parameters given the prespecified logic templates and the input event data.

Logic templates introduced here look like: 

# For example, consider three rules:

    # A and B and Equal(A,B), and Before(A, D), then D;
    
    # C and Before(C, Not D), then  Not D
    
    # D Then  E, and Equal(D, E)

# Note that in this simple demo example, we assume the base transition intensity term for 0 --> 1 and 1 --> 0 are the same (just for simplicity of demonstration). 
In practice, the base transition intensity of for 0 --> 1 and 1 --> 0 can be quite different. We can just introduce more base variables to indicate this.
