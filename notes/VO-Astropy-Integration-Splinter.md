This document:  [http://bit.ly/spssa18-voastropy](http://bit.ly/spssa18-voastropy)

Seed presentation:  [https://stsci.box.com/s/9wkbu73e0qz8mtw57m0xio4pvlps141b](https://stsci.box.com/s/9wkbu73e0qz8mtw57m0xio4pvlps141b)

Astroquery is considering:

What are the boundaries between astroquery and PyVO?

AQ may not actually want to be more tightly coupled.

Astroquery.gaia.tap ([https://astroquery.readthedocs.io/en/latest/gaia/gaia.html](https://astroquery.readthedocs.io/en/latest/gaia/gaia.html))

Astroquery.utils.tap ([https://astroquery.readthedocs.io/en/latest/utils/tap.html](https://astroquery.readthedocs.io/en/latest/utils/tap.html))

LSST’s recommended access to images is through Bulter.  Catalog access is less clear.

LSST would like for there to be a robust VO library for accessing their collections (TAP, SODA, etc.)

Interested in building a group of people who know both VO and astropy ecosystem deeply enough.

Astroquery by design is supposed to be able to support looping over all modules.  Given a choice between that, and a similar VO option, what would a user want to do?  Can we influence that?  Should we, or should we instead just be driven by user demands?

Maybe the “virtuous” plan is to use the VO as an “underlying” technology that’s mostly/entirely hidden from the astronomer user.

  
  

Building server-side libraries is also potentially useful to prime the pump of usefulness.  Containerized data server deployment, for example, is now possible.

Some discussion of data models, and even auto-discoverable mappings to models for catalog tables.

Simple semantic example would be for astropy to interpret the RA/Dec as a skycoord.  MAST Portal and Aladin do this.  This would be a great first step and probably low-hanging fruit.



We agree that there is a need for a robust Python library API to access VO services across various data sources.
