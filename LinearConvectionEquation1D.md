# Solve the Navier-Stokes system using CFD model in Python;
# Trying to improve my research about climate changes and the dynamic of the southern pacific ocean, I'm trying to apply this model to solve the Navier-Stokes equations, which will be very useful in my research;
# This model uses the 1D linear convection equation to training

import numpy as np
from matplotlib import pyplot
import time, sys

domain = np.linspace(0., 2., num = 51) # Graphic domain
nsteps = 100 # time steps number
tsteps = .025
c = 1 # Wave velocity
nx = x.size # Number of points to the iteration
dx = x[1] - x[0] # Differenciation

# Now we define the initial conditions of the problem
u = numpy.ones_like(x)
u[(1,03<=x) & (x<=1.53)] = 2
print (u)

# Then we use the pyplot library to require the graphic
pyplot.plot(x, u);
# Where un is the u value on the iterations
un = numpy.ones_like(u)

for n in range(nt):
    un = u.copy()
    for i in range(1, nx):
u[i] = un[i] - c * dt / dx * (un[i] - un[i-1])

# Plotting the space x velocity chart
pyplot.plot(x, u):

...
