# NumericalEarth

<p align="center">
  <strong>Open-source tools for simulating the Earth system at all scales</strong>
</p>

<p align="center">
  <a href="https://numericalearth.github.io/NumericalEarthDocumentation/dev">Documentation</a> |
  <a href="https://github.com/NumericalEarth/NumericalEarth.jl/tree/main/examples">Examples</a> |
  <a href="https://github.com/orgs/NumericalEarth/discussions">Discussions</a>
</p>

NumericalEarth is a community building Julia software for Earth system modeling. We develop tools for running coupled atmosphere-ocean-sea ice simulations, wrangling climate datasets, and studying boundary layer physics --- from turbulence-resolving large eddy simulations to global climate models.

The NumericalEarth organization is anchored by an Earth system modeling package called `NumericalEarth.jl`.
`NumericalEarth.jl` is in turn built on [Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl).
Our core mission is to accelerate progress in Earth system modeling, utilizing a strategy that combines ground-breaking user interface design with
algorithms and numerical strategies that maximize both GPU performance and accessibility to scientists.

<p align="center">
  <img width="1920" height="1080" src="https://github.com/user-attachments/assets/448c5c86-aa6f-4e36-86ef-6463d14294b0" alt="Global ocean-sea ice simulation" width="80%" />
  <br />
  <em>Ocean surface speed and sea ice speed in a coupled ocean-sea ice simulation on a 1/6th degree tripolar grid (<a href="https://github.com/CliMA/Oceananigans.jl">Wagner et al. 2025</a>)</em>
</p>

<p align="center">
  <img width="1920" height="1080" alt="moist_baroclinic_wave 001" src="https://github.com/user-attachments/assets/46cb1ebd-1984-4cad-98df-460a50ee2467" />
  <br />
  <em>(Left) Atmosphere vertical integral of total liquid density and (right) surface speed in a simulation of moist baroclinic instability with prescribed SST and on a 1/24th degree latitude-longitude grid spanning 80 S, 80 N</em>
</p>


## Getting Started

- Read the [Documentation](https://numericalearth.github.io/NumericalEarthDocumentation/dev) for guides and tutorials
- Browse the [Examples](https://github.com/NumericalEarth/NumericalEarth.jl/tree/main/examples) for runnable scripts
- Install the main package:
  ```julia
  using Pkg
  Pkg.add("NumericalEarth")
  ```

## Projects

### Core Framework

- [NumericalEarth.jl](https://github.com/NumericalEarth/NumericalEarth.jl) --- Coupled Earth system modeling with prescribed or prognostic atmosphere, ocean, sea ice, and land components
- [Breeze.jl](https://github.com/NumericalEarth/Breeze.jl) --- Limited area LES-to-mesoscale atmosphere simulations based on Oceananigans
- [Terrarium.jl](https://github.com/NumericalEarth/Terrarium.jl) --- Global and regional land and terrestrial ecosystem modeling (soil, vegetation, snow, hydrology) at all scales

### Data and Tooling

- [CopernicusMarine.jl](https://github.com/NumericalEarth/CopernicusMarine.jl) --- Julia wrapper for the Copernicus Marine Service
- [CopernicusClimateDataStore.jl](https://github.com/NumericalEarth/CopernicusClimateDataStore.jl) --- Julia wrapper for accessing ERA5 data through the Copernicus Climate Data Store
- [XESMF.jl](https://github.com/NumericalEarth/XESMF.jl) --- Julia wrapper around xESMF for conservative regridding
- [pynanigans](https://github.com/NumericalEarth/pynanigans) --- Shenanigans and Oceananigans in Python

### Research and Learning

- [PolarPlunge.jl](https://github.com/NumericalEarth/PolarPlunge.jl) --- Julia, GPU and fluid dynamics tutorial with Oceananignans and SpeedyWeather
- [SwimLessons.jl](https://github.com/NumericalEarth/SwimLessons.jl) --- Tutorials that teach ocean-flavored fluid dynamics with Oceananigans
- [Cumulography.jl](https://github.com/NumericalEarth/Cumulography.jl) --- The art of cloudmaking
- [DataAssimilocean.jl](https://github.com/NumericalEarth/DataAssimilocean.jl) --- Experiments in ensemble-based and variational data assimilation

## What Can You Do With NumericalEarth?

**Coupled global simulations** --- Run ocean-sea ice models forced by atmospheric reanalysis (JRA55, ERA5), or fully coupled atmosphere-ocean experiments with [SpeedyWeather.jl](https://github.com/SpeedyWeather/SpeedyWeather.jl)

**Boundary layer research** --- Study atmosphere-ocean interactions through Monin-Obukhov similarity theory, bulk flux formulations, roughness length models, and sea surface albedo schemes

**Climate data wrangling** --- Download, cache, regrid, and interpolate datasets from ECCO, GLORYS, ERA5, JRA55, EN4, and ETOPO bathymetry into model-ready formats

**High-performance computing** --- Leverage GPU acceleration for global simulations

## Contributing

We welcome contributions! Whether you're fixing bugs, improving documentation, or proposing new features, check the issues in the relevant repository to get started.

Questions or ideas? Open a thread in our [Discussions](https://github.com/orgs/NumericalEarth/discussions).

## Community

Join the [NumericalEarth slack](https://join.slack.com/t/numericalearth/shared_invite/zt-3pwpvky4k-XX7RkgQgHLIUt~wtwGXN~Q) to connect with the NumericalEarth community!
