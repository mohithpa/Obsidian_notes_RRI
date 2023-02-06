GMOSS: Global Model of the Radio Sky Spectrum.

## Abstract: 
- To model the low frequency Radio sky.
- Works on frequency: 22MHz to 23 GHz.
- Invokes physical components and radiative processes rather than data driven unlike GSM.
- describe the sky spectrum over 3072  pixels of 5$\degree$  resolution.
 Contributions to spectrum are from: 
 - Thermal emission 
 - Synchrotron emission
 - free - free absorption? [[Bremsstrahlung radiation]]
Physical parameters are controlled by 4 all sky maps and we fit the parameters to those sky maps.
--> Aimed at modelling foregrounds for the global signal arising from the 21-cm line of Hydrogen during Cosmic Dawn and Epoch of Reionization (EoR) from the red - shift (150<z<6).
- The complexity in spectral structure that naturally arises from the underlying physics of the model provides a useful expectation for departures from smoothness in EoR foreground spectra

# Introduction
Radio sky:  -> 
- It is now understood that the predominant  
radiative mechanism contributing to this Galactic emission at long wavelengths is synchrotron radiation from relativistic electrons spiraling around Galactic magnetic field lines.

radio sky has the following sources in general
1. signals from our galaxy
2. extragalactic radio sources
3. Cosmic Microwave background([[CMB]]) 
+
Added spectral distortions related to thermal history of baryons , structure formation, energy release in the early universe and interactions between propagating radiation and gas.(These include distortions from Cosmic dawn and Epoch of Reionizaion [[EoR]]).

[[Spin Temparature]]
A fictitious temperature that describes the average spin of neutral hydrogen (H I) atoms in a gas cloud. H I has two energy states: an upper state in which the spins of the electron and proton are parallel, and a lower state in which the spins are opposite (_antiparallel_). The spin temperature of an H I region is the temperature that would produce the observed ratio of parallel to antiparallel spins if the H I gas were in thermal equilibrium. The transition between the two spin states of the H I atom produces the important radio spectral line at 21 cm wavelength.

The 21 cm emission are a probe of the thermal history of the gas

- (->==Microwave frequency is from 300MHz to 300Ghz==).

There are global, all-sky isotropic spectral features as well as angular variations in spectral structure, embedded as tiny additive components   in the radio background at frequencies . 200 MHz. Radio emission from Galactic and extragalactic sources forms strong foregrounds to the cosmological signal and are orders of magnitude brighter.

What is Wouthusen-Field coupling of spin to kinetic temperature ??
- SED: (Spectral Energy Distribution)

- Waelkens et al present a tool to simulate maps of the total and polarized synchrotron emission of the radio sky including effects of Faraday rotation.
- Global sky model: (GSM): de Olivera-Costa et al. and improvements were made by Zheng et al. use data driven methods to generate snapshots of the sky at frequencies between those where large area maps are available.  -> Worst in in error <= 10% depending on the region of the sky.
what is a $cos^2$ antenna beam?
What is mono energetic cosmic ray?

GMOSS: Not exactly a data driven model but rather a physical process driven model (mainly synchrotron radiation etc.)

In GMOSS we present a physical sky model that includes effects of plausible radiative processes arising from different components of the radio sky. Additionally, physical parameters used to describe GMOSS are guided by all-sky maps at different frequencies, thus enabling a check on the goodness of the model.
- what is spectral index?

The sky maps used in GMOSS are 150MHz, 408MHz, 1420 MHz and 23 GHz.

GMOSS Physics: 

The dominant emission of low radio frequency is ==synchrotron radiation==. The $\gamma$ factor ([[gamma factor]])  

Go through Rybicki and Lightman for detailed treatment of synchrotron radiation.

Downhill simplex algorithm: Also called [[Nelder-Mead method]] / amoeba method or polytope method.

[[Link and resources]]  
https://machinelearningmastery.com/curve-fitting-with-python/

$\alpha$  in  

- try to make better educated guesses(go through the numerical recipes in fortran book )
- also try changing the data so as to match the pts and do vice versa. We can look at the parameters later
- get the curve to fit first.
