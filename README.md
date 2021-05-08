# RSP
Modules folder:

Contains the different parts of the project. These are:

1. **Network** generator
2. **Gillespie** solver
3. **Parsing+Statistics** utility toolkit

The modules are listed in logical order. First a subtree of reactions is generated via *Network* and converted into a set of kinetic equation for the extended two state model. This set of equation is then plugged and solved by *Gillespie* and written into .txt file (.csv eventually possible). The .txt files are then read, parsed and analyzed by the *Parsing+Statistics* toolkit.

