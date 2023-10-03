# Simulating the Universe: Using Latent Diffusion Models to Create Cosmological Data

This model is based on Alex Zhou et al's Point Voxel Diffusion Model, found here: https://github.com/alexzhou907/PVD. Their paper can be found here: https://arxiv.org/abs/2104.03670. 

The abstract from my paper outlining this project is below: 

Machine Learning models, particularly generative models, are capable of creating ever more realistic data, with a wealth of possible applications. One such application is in assisting and accelerating cosmological research. Cosmology relies on simulations to create data that provides statistically accurate results, in order to corroborate current theory to observations. The caveat is that the computational cost required to create the data is high, requiring a large amount of time and sufficiently adequate hardware to be of much use to the field. This paper demonstrates that diffusion models, a class of generative models, are capable of emulating the data from these simulations at a fraction of the time taken, with fairly accurate results, for both two and three dimensional data. By emulating the simulated data, the volume of the total data available to use for statistical comparisons can increase at a rapid rate, which will allow cosmological research to have more resources to draw from. 

Some key results are included in the results directory, such as the raw 10000th epoch png file for the linear and cosine noise schedules, as well as the graphs of the main results.

To run the code with optimal parameters:

```
$python3 path/to/folder/tgq.py --niter 10000 --workers 12 --schedule_type 'linear'
```

Dataset required: Quijote Simulations, processed as in PVD Dataset Creation and Visualisation.ipynb

Link to dataset: https://drive.google.com/file/d/1n4w60eEdlIu2veO8TfQ8OxTtTkWSvuJ2/view?usp=drive_link 




