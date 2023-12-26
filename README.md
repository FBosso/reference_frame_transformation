# Geodetic Coordinates Transformation
<a href="https://mapflap.github.io"><img align="right" src="https://i.ibb.co/NspjQxV/logo.webp" alt="logo" width="220"></a>

## Overview

*This repository contains Python code to solve the problem of transforming geocentric ITRS Cartesian coordinates of COMO PS to geodetic coordinates in the ETRF reference frame. The transformation involves multiple steps, including ITRF baselines, local network surveys, and conversions to the Local Level reference system. The final output provides geodetic coordinates for points BRUN, 0001, 0002, and 0003 at February 2nd, 2019, along with standard deviations.*

## Author
[Bosso Francesco](https://github.com/FBosso) - (fra.bosso97@gmail.com)

## Problem statement
* COMO PS in EPN: COMO PS belongs to EPN, and its geocentric ITRS Cartesian coordinates are available on the EPN website, using IGS14 = ITRF14 estimates.
* ITRF Baselines: 
	* The ITRF baseline from COMO to BRUN has been measured at February 2nd, 2019 
	* Local network baselines from BRUN to point 0001 are also available.
* Local Network Survey: 
	*A local network composed of points 0001, 0002, and 0003 has been surveyed around BRUN 		using terrestrial instrumentation 
	*Estimated accuracies for the coordinates are σXLL = 10 cm, σYLL = 10 cm, and σZLL = 15
	cm.
* Transformation and Computation:
	* The Python code transforms the coordinates and computes the geodetic coordinates (latitude, longitude, and geodetic height) of BRUN, 0001, 0002, and 0003 in ETRF at February 2nd, 2019.
	* Standard deviations of the geodetic coordinates are also computed.

<img src="problem_schematics.png" alt="plot" width="100%">

## Dependencies
This project relies on the following libraries:

+ [numpy](https://numpy.org/): Used for array operations.

```bash
$ pip install numpy
```




## Usage
To run the project, make sure to install the required dependencies mentioned above. Then, execute the script "main.py"