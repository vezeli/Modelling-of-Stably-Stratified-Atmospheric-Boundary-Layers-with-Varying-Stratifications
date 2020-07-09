
.. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.3937500.svg
   :target: https://doi.org/10.5281/zenodo.3937500

This repository contains data that was used for publishing article
called `Modelling of Stably Stratified Atmospheric Boundary Layers with
Varying Stratifications <https://doi.org/10.1007/s10546-020-00527-8>`_.
The repository compliments the publication in the sense that it provides
qualitative insight for comparison and exploration.

**Keywords**: GABLS1, Open data, Stably-stratified turbulence,
Turbulence parametrization, 

Data Structure
==============

The data is stored inside sixteen files. The file names are split into a
part that describes variables and part that describes simulation. Here's
an example of a file name::

  budgets.cr0375.csv

The first part ``budgets`` refers to variables inside the file and the
second part ``cr0375`` refers to forcing conditions (in this example
cooling rate of 0.375 Kelvin per hour) used in the simulation.

Variables:

* ``first_order_stat`` <- contain mean wind speed and mean potential
  temperature

* ``second_order_stat`` <- contain variance and covariance variables
  that describe turbulence properties

* ``budgets`` <- contain variables used in the turbulent kinetic energy
  and half the temperature variance equations

* ``lambda_beta_coeffs`` <- contain values for model coefficients that
  can be used for calculating second order statistics

Simulations:

* cooling rate at the surface 0.25 Kelvin per hour -> ``cr025``

* cooling rate at the surface 0.375 Kelvin per hour -> ``cr0375``

* cooling rate at the surface 0.5 Kelvin per hour -> ``cr05``

* cooling rate at the surface 1.0 Kelvin per hour -> ``cr1``

**Note**: The results presented in the repository are taken after the
ninth hour of the simulation while the results in the published paper is
averaged between the eight and ninth hour. This difference should be
negligible.
