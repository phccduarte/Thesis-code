# Thesis-code
In this repository, you can find some of the code and models I developed for my Master's Thesis (https://drive.google.com/file/d/14Co0BssyLrfycW10g6ck5IVyVc_7s-fe/view). I did not upload the data because of data permissions, so, other than the simulations, it is not possible to run the files. However, their outputs can be seen in the notebooks. (If you'd like to run the code, I can try to get the permissions)

There are three folders: 1)fits_code ; 2)sims_code; 3)abc_code.
The first one contains the code for the analytical solution for cascade growth (the model is explained in section 3.2 of the Thesis). The second one contains the code for the simulations. The third one contains the code for the search of the combination of parameters that best describes the data, using Approximate Bayesian Computation.
Each of these are further described in the sections below.

## fits_code - Analytical Solution for Cascade Growth
In fit_cascades.ipynb, our model is applied to every cascade in the dataset (the cascades were assembled previously from the raw data).
In cascades_examples.ipynb, you can see a few examples of cascades and their fit, using our model.
Finally, in histofram_parameters.ipynb, you will find histograms for each of the parameters of the fitting model. For each dataset, hundreds of thousands of cascades were analyzed.

## sims_code - Simulations
In sim_v13.ipynb, you will find the final version of our model for the simulated diffusion of information in a network. It is fundamentally a SI model, but its specificities can be found in section 3.3.
In sim_cascades.ipynb, you can find a few examples of the growth of the simulated cascades.

## abc_code - Approximate Bayesian Computation
Our simulations have 4 input parameters. To find out which combination produced the same distribution of cascade sizes as the one from the data, we use used Approximate Bayesian Computation. This can be found in abc.ipynb.
