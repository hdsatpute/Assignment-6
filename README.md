# Assignment-6

# Stress When depth is constant
Q = float(input("Enter the value of Load in kN: "))
N = int(input("Number of data values of radial distance: "))
Z = float(input("Depth: "))
r = []
for i in range(1, N + 1):
   print ("Enter radial distance in m".format (i))
   Value_r = float(input () )
   r.append(Value_r) # this line was not indented correctly, causing the error
   Stress = ((3*Q)/(2*math.pi*Z*Z) ) * (((1/ (1+((Value_r/Z) **2))) ) ** 2.5) # Q was missing and pi needs to be called from the math module
   print ("Stress: ", Stress, " kN/m^2")
