# trisurf-ng
my fiddling with trisurf-ng by samo and miha  
Adding a CMC-CMC Vicsek-style interaction, new tape parameter "vicsek_strength"



The direction of the force on each vertex is directed by a weighted sum  
```
F = (1/vicsek_strength)×Normal + sum(neighbors normal)
```
Setting vicsek_strength=0 gets us back to the regular trisurf (special case, no division by 0, mathematically this is equivalent due to normalization)
