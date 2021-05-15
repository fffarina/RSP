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

 - [x] Network module:
   - [x] Generate random weighted, undirected graph
   - [x] Define subset of possible shortest paths via BFS
   - [x] Convert found paths into kinetic reactions
   - [x] Store kinetic reactions in dictionaries

 - [ ] Gillespie module:
   - [x] Constrain simulated trajectories into fixed amount of timesteps
   - [ ] Fix internal logic of the program in order to:
         - [ ] Not interrupt simulation if no reactions found
         - [ ] Don't allow negative species populations
         - [x] Avoid usage of reserved words like "time" in dictionaries
   - [ ] Write time steps, species counts and propensities into .txt file
   - [ ] Store time steps, species counts and propensities into list of arrays

 - [ ] Parsing+Statistic:
   - [ ] Write statistics per simulated trajectories into .csv files