# particle-swarm-optimization

Comparison of different implementations of Particle Swarm Optimization in the context of high-performance computing

Particle Swarm Optimization is a population-based optimization algorithm inspired by social behavior. It's highly parallelizable and effective for continuous optimization.

The idea behind this technique is to initialize a population (called a swarm) of candidate solutions (called particles) which are represented with vectors of numeric values, which can be considered as coordinates of points in a search space. The next position of a particle is determined by its best position yet, the best position yet of the whole swarm and several population parameters. These parameters are used to calculate the velocity of each particle using the following formula:

v = v * w + c1 * r1 * (pb - p) + c2 * r2 * (gb - p)

Here the parameters are:
- v - the current velocity
- p - the current position
- w - the inertia weight
- c1 - the cognitive coefficient
- c2 - the social coefficient
- pb - the personal best position
- gb - the global best position
- r1, r2 - random coefficients

Link to the CUDA implementation: https://colab.research.google.com/drive/1WNmk3DYI8oSVNpPJY97nZDGlVL-nkznG?usp=sharing