---
layout: post
title:  "Computational Magma Ocean Modeling"
date:   2018-07-18
excerpt: "Iron Rain in Magma Oceans...How to Interpret Mantle <sup>182</sup>W Abundances?"
project: true
tag:
- exoplanet
- pocketknife
- habitable
- tectonics
- modeling
comments: true
---

# The Terrestrial Magma Ocean...Birth of a Planet!
Terrestrial planetary accretion is a violent and energetic process.  So energetic, in fact, that most of the new planet should remain molten for millions of years.  
This length is up for debate due to the large number of unknowns involved with magma oceans (notably the presence and composition of a potential primitive and insulating atmosphere), but 
the release of gravitational energy through viscous dissipation of stratifying phases and the decay of short-lived isotopes (<sup>26</sup> especially) should keep the planet above silicate soldii for 
a geologically significant amount of time.  Moreover, the planet may melt more than once.  On Earth, the moon-forming impact may have marked the last presence of at most a shallow magma ocean on 
the surface of the planet.  The rate of cooling and chemical stratification in Earth's magma ocean are critical areas of research, since they should set the initial conditions for the formation of the planet 
and control the geologic outcome of the planet.

# The Iron Rain Hypothesis
Iron is highly abundant within the Earth.  33% of the Earth's mass is found in the dominantly-iron core.  It is thought that one route of core formation for planets like Earth is the <sup>iron rain hypothesis</sup>.  
Iron is immiscible with silicate liquid and gravitationally unstable, foundering with the magma ocean and sinking as droplets to the center of the planet to form the core (also releasing gravitational energy through viscous dissipation).  
Isotopic fingerprints of this process are thought to exist within the Earth's mantle (the remnants of the magma ocean which fell below the silicate liquidus).  The <sup>182</sup>Hf/<sup>182</sup>W isotope system is especially curious, 
as lithophile <sup>182</sup>Hf (half-life ~ 9 million years) decays to moderately siderophile <sup>182</sup>W.  The idea is that any <sup>182</sup>Hf extant during the magma ocean's lifetime would have decayed to 
<sup>182</sup>W, which would partition to the sinking iron droplets.  After the magma ocean cooled, the remaining <sup>182</sup>Hf would still decay to <sup>182</sup>W and constitute the modern mantle's <sup>182</sup>W budget.  
Using this knowledge, one may reconstruct the lifetime of the terrestrial magma ocean!  However, there is much ambiguity in this process.  Current analytical solutions are greatly simplified, and there is <sup>182</sup>W heterogeneity in 
<sup>182</sup>W measurements from Earth's mantle that obscures the mantle standard <sup>182</sup>W abundance.  Furthermore, partitioning behavior of <sup>182</sup>W in magma ocean conditions in poorly constrained.  Therefore, my work takes 
the methods of [Rubie et al. 2003](https://www.sciencedirect.com/science/article/pii/S0012821X02010440) and expands them in much more detail within a numerical computational environment.

# Meet Chimera!

![Iron Droplets Descending & Interacting as Modeled by _Chimera_](/assets/img/posts/plot_cell_therm.gif "Iron Droplets Descending & Interacting as Modeled by Chimera")

_[Chimera](https://github.com/ScottHull/Chimera/tree/develop/Chimera)_ is my Python-based 3D two-phase flow software package that supports thermal and chemical diffusion in a user-defined box model over user-defined 
timescales.  It is named after the mythical monstrous hybrid beast, which seems appropriate given all that <i>Chimera</i> can do (the bad omen part of the myth is for me).  For my Master's thesis, I will use Chimera 
to model <sup>182</sup>W partitioning to sinking iron droplets in a magma ocean.  This numerical approach should shed light on the continuum behavior of <sup>182</sup>W partitioning to sinking iron droplets within 
a magma ocean.  <i>Chimera's</i> support of parameter gradients and droplet density variation will allow the model to behave as realistically as possible within performing outside of reasonable computational time.  
Chimera also allows the droplets to only interact with the local environment, so chemical gradients may result from the model as well.

