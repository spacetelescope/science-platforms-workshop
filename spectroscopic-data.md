# Spectroscopy on Science Platforms

Was: Spectroscopic Data in Jupyter

Auditorium, 2018-02-26, 15:30-16:30.

## General Ideas Related to Spectroscopic Data

These are things that we just "want to do".

* (Specviz)[https://github.com/spacetelescope/specviz] → Jupyter?
  - STScI is roadmapping this
* Look at many spectra
  - STScI is working on mosviz
* Pipelineable extractions?
  - Idea is to have specutils + specreduce support this.
* Flux versus wavelength in a NoSQL database, *e.g.* MongoDB?
* Cubes!
  - Ask JHU/SciServer whether a Marvin demonstration might be possible.
  - Cubeviz for JWST is being developed.
  - Some cubes may be more generic than others.
* Stellar parameters, *e.g.* (The Cannon)[https://arxiv.org/abs/1501.07604].

## Priorities

What things should we focus on?

* Just press the "Science" button!
* Generic interactivity, and low-level analysis tools.
  - EW, addition, manipulation
* User says "I want splot."
  - Developer says "There’s a better way."
  - Automate the intuitive, exploratory aspects of tools like splot.
  - Can we "capture" aspects of how users perform analysis?
    - This is potentially "creepy", but easy automation is generally a good thing.
* How different do the tools need to be as you move away from UVOIR spectra, in both directions?
* Work with lab spectra as well as on-sky.
* Simulate spectroscopic surveys, *e.g.* (DESI)[https://github.com/desihub/two_percent_DESI].
  - Use the platform as a testbed.
* Follow up for TESS, other surveys.

## Science Platform Specifics

What can we do on a Science Platform that we can't do on a laptop?

* There’s 1e7 spectra.
* Aggregate different instruments so there’s one platform, not seven…
* Aggregate many different wave bands.
* Combine catalog data with flux versus wavelength.
* Look back at imaging data.
* Look at temporal variation.
  - Could be lots of this in the future.
  - Cross-correlation can get intensive.
