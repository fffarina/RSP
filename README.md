# RSP
Modules folder:

Contains the different parts of the project. These are:

1. **Network** generator
2. **Gillespie** solver
3. **Parsing+Statistics** utility toolkit

The modules are listed in logical order. First a subtree of reactions is generated via *Network* and converted into a set of kinetic equation for the extended two state model. This set of equation is then plugged and solved by *Gillespie* and written into .txt file (.csv eventually possible). The .txt files are then read, parsed and analyzed by the *Parsing+Statistics* toolkit.

The intended Input / Output datatypes are as follows ( Input / Output):

1. **Network**: User defined / Dictionaries
2. **Gillespie**: Dictionaries / .txt files & list of arrays
3. **Parsing+Statistics**: .txt files & list of arrays / plots & .csv files

TO DO LIST:

 - [] Network module:
   - [] Generate random weighted, undirected graph
   - [] Define subset of possible shortest paths via BFS
   - [] Convert found paths into kinetic reactions
   - [] Store kinetic reactions in dictionaries

 - [] Gillespie module:
   - [] Constrain simulated trajectories into fixed amount of timesteps
   - [] Write time steps, species counts and propensities into .txt file
   - [] Store time steps, species counts and propensities into list of arrays

 - [] Parsing+Statistic:
   - [] Write statistics per simulated trajectories into .csv files