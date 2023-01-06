# SIR-Model-in-R
SIR Model for disease transmission in closed population in R


Parameters
β	is the transmission rate and incorporates the encounter rate between susceptible and infectious individuals together with the probability of transmission.
γ	is called the removal or recovery rate, though often we are more interested in its reciprocal (1/γ) which determines the average infectious period.
S(0)	is the initial proportion of the population that are susceptible.
I(0)	is the initial proportion of the population that are infectious.



We have 3 variables S, I and R which are respectively the numbers of susceptibles, infectious and recovered, and we have 2 parameters β and γ which are respectively the infectious contact rate and the recovery rate.

A mathematical description
A mathematical description of the above SIR model using the differential equations formalism looks like:

dS/dt=−β×I×S
dI/dt=β×I×S−γ×I
dR/dt=γ×I

The basic reproductive ratio R0 for this system is

R0=βγN

FIND CODE IN THE FILES 


###########################################
#    SIMPLE SIR MODEL BY DR.ABDUL ALI     #
###########################################

#Description of Model - SIR

#S susceptibles, I infectious and R recovered. Susceptibles become infected at a rate equal to the product of an infectious contact rate β and the number of infectious I. Infectious people recover at a rate γ.

#PACKAGES REQUIRED ARE - ggplot, rehshape2 and deSolve, if these packages are not installed, please install them with simple command as install.package("packagename")
