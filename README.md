# Science Platforms/Server-Side Analytics Workshop

### What
Building upon the [strong interest](https://www.youtube.com/watch?v=eEBbqyagNUI&feature=youtu.be&t=8h4m40s) of the community at ADASS 2017 in 'Science Platforms/Server-Side Analytics', STScI is hosting 2.5 day meeting with a focus on sharing community approaches to science platforms, documenting common data analysis patterns/workflows, identifying challenges different implementers are facing and prototyping solutions to address these challenges.

## When
26--28 February 2018

## Where
[STScI](http://www.stsci.edu) in Baltimore, MD.

## Remote participation

We will have WebEx sessions available for remote participants to listen in, 'full' participation of remote people is not planned however (i.e. don't expect to be able to ask questions during talks).

See [remote instructions](remote.md) for more information.

## Registration
Registration is $140. This charge will cover catering costs for the three days. There may be a small amount of travel support available upon request.

The conference registration site is here: https://www.eiseverywhere.com/ereg/index.php?eventid=310200

## Organizers

Arfon Smith (STScI), Wil O'Mullane (LSST), Adam Bolton (NOAO), Gregory Dubois-Felsmann (IPAC), Gerard Lemson (JHU)

## Agenda

An up to date agenda is available here: https://docs.google.com/spreadsheets/d/1hTjg-8537Te8eF2_R-VZHxu0dekFWymf3abP4pN4zwY/edit#gid=0

## Format
The goal is to have a collaboration workshop where:
- Engineers share their experiences and work together on technical solutions to common challenges and...
- Astronomers are in the rooms and are able to share common use cases/data analysis workflows that can be used to ensure we're building tools of value to the scientific community.

The format will be to have short lightning talks each morning aimed at a particular topic area (see below) and for the remainder of the day to be spent in smaller groups discussing implementation ideas and prototyping solutions. Each day will close with different teams reporting back on progress they have made that day.

Examples of topic areas likely to be covered in this workshop include:

- Use cases & user experience: What sorts of scientific use cases do science platforms make possible? What use cases are different centers considering supporting? What is out of scope for each center?
- Authentication, authorization: How are different groups authenticating and authorizing users? This includes authenticating between different services and applications
- Data models
- User workspaces, user quotas and publishing data: What approach are people taking for allocating resources to individuals and groups. How are we all thinking about long-term hosting of data.
- Batch processing: What approaches are different groups taking for providing access to batch compute resources?
- Interoperability and open standards: How are different centers thinking about interoperability. What combination of approaches are people using e.g. VO services, client libraries etc. What technologies can we standardize/agree on now if any? Shared continuous integration (CI) frameworks and joint containers (e.g. containers with LSST/JWST pipeline software)
- Community contributions: What approach are different centers taking for incorporating community contributions? This includes contributions to core technologies used in science platforms, pipeline software for batch processing of data, community contributed virtual machines/containers and more...
- Deployment: What tools and technologies are different groups using for deployment of their science platforms


## Questions?
Feel free to [open an issue](https://github.com/spacetelescope/science-platforms-workshop/issues/new) here on the workshop GitHub repository or email LOC lead Arfon Smith on arfon@stsci.edu
