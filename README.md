# Constants

This repo contains a dictionary of common physical and mathematical constants.
It is meant to be used inside E3SM and related projects, to ensure that all components and tools agree on the
numerical value of such constants.

The yaml file is organized in sections, which are meant to contain constants of a certain category. For instance,
`pi` or `e` are _mathematical_ constants, the speed of light or the Boltzmann constant are _phisical_ constants, while the Earth radius or the gravity acceleration on earth surface are _geophysical_ constants.

Within each section, constants are listed as maps (in the YAML sense). Each constant contains the following fields:

- name: a short name for the constant
- symbol: a symbol compatible with cxx/f90 source code ([a-zA-z0-9_] only, not starting with a number)
- value: the numerical value of the constant
- units: the fundamental SI units of the constant (or 'none' for dimensionless units)
- description: a detailed description of the constant
