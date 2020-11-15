Benchmark-Ph1Ex2:
-----------------

[1]
Exercise 2 defines a thermal-fluids standalone calculation.
It specifies the power density in the fuel region.
This exercise's purpose is to ensure that the thermal fluid model differences between participants are negligible and that it will not affect the coupled exercises.

Four sub-cases compose exercise 2:
* 2a: No bypass flow and fixed thermophysical properties. There is no bypass flow. The thermo-physical properties are constants.
* 2b: Bypass flow type I and fixed thermophysical properties. This exercise prescribes the bypass flow distribution. The thermo-physical properties are constants.
* 2c: Bypass flow type I and variable thermophysical properties. This exercise prescribes the bypass flow distribution. The thermo-physical properties depend on different simulation parameters.
* 2d: Bypass flow type II and variable thermophysical properties. This exercise solves the bypass flow distribution through the explicit modeling of the bypass gaps. The thermo-physical properties depend on different simulation parameters.

Fixed thermopysical properties:
Material 				Conductivity
Fuel compact				20
Fuel block 					37
Grade H-451 graphite 		66
RPV							40
Coolant						0.41
Air 						0.068

The primary parameters of interest for Exercise 2 are the gas and solid temperatures and global parameters such as the pressure drop over the core and the inflow mass flow rate.
The benchmark requires participants to also report secondary parameters such as the calculated thermal conductivities, mass flow rate or velocities in bypass channels and heat transfer factors.
This data is helpful to trace the source of possible differences in the primary parameters.
Only a subset of available data will be presented to illustrate the main characteristics for each of the Exercises.

			R1	R2	R3
helium temp 797 636 673
fuel temp 	863 688 722
mode temp 	843 672 not shown, 690-730

Firs ring:

   fuel temp
L1 	864
L2	847
L3	824
L4	796
L5	767
L6	739
L7	699
L8	645
L9	568
L10	460

[2]
Plot with axial temperatures of all the rings

[3]
Table I.10. Thermal-fluids boundary conditions.

The benchmark provides a file with a fluence map for evaluating the thermo-physical properties.

Reporting:
- fuel temperature
	- average
	- max
- heat flux (RPV): all surrounding surfaces
- fluid temperature
	- channels: average and max
	- bypass: average
	- average outlet helium temp
- mass flow rate distribution in channels and bypass
- moderator temperature
	- average
- reflector temperature
	- average
- RPV temperature
	- max


Benchmark-Ph1Ex3:
-----------------

[1] Section 6. Results for ex3.
3a) CR nominal, CR all out, CR all in.
3b) CR nominal, CR all out, CR all in.

[2]
Exercise 3 combines all the data from the first two exercises, and the participants need to determine a coupled neutronic and thermal fluids solution.
Cross section updates are performed for four state parameters: moderator and fuel temperature, xenon-135, concentration and the hydrogen concentration.
In addition to this data, the benchmark requires the use of fluence maps to determine the thermal therm conductivity of graphite, as well as the implementation of a set of design-specific design thermophysical material properties.

[2]
Coplued calculation: 2 energy group structure: parameters: Diffusion coef, absorption, scattering, fission.
keff=1.0243 (CR not model)

[3]
Two sub-cases:
- Exercise 3a: based on exercise 2c.
- Exercise 3b: based on exercise 2d.

References:
-----------
[1] INL results for Phases I and III of the .... 2013.
[2] Strydom et al. RELAP5-3D results for phase I (Exercise 2) of the OECD/NEA MHTGR-350 MW benchmark. 2012
[3] OECD/NEA. Benchmark ...