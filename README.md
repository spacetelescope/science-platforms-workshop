# Science Platforms/Server-Side Analytics Workshop

### What
Building upon the [strong interest](https://www.youtube.com/watch?v=eEBbqyagNUI&feature=youtu.be&t=8h4m40s) of the community at ADASS 2017 in 'Science Platforms/Server-Side Analytics', STScI is hosting 2.5 day meeting with a focus on sharing community approaches to science platforms, documenting common data analysis patterns/workflows, identifying challenges different implementers are facing and prototyping solutions to address these challenges.

## When
26--28 February 2018

## Where
[STScI](http://www.stsci.edu) in Baltimore, MD.

## Registration
Registration is $140. This charge will cover catering costs for the three days. There may be a small amount of travel support available upon request.

The conference registration site is here: https://www.eiseverywhere.com/ereg/index.php?eventid=310200

## Organizers

Arfon Smith (STScI), Wil O'Mullane (LSST), Adam Bolton (NOAO), Gregory Dubois-Felsmann (IPAC), Gerard Lemson (JHU)

## Agenda

### Day 1 (26 February, 2018)

The goal of the first day is for all of the science platform implementers to share what they are building, discuss the sorts of use cases they’re designing for (e.g. survey query services, batch processing, hosted data analysis environment for small amounts of data). Each group will be also asked to give a brief overview of the technologies they’re using, major technical challenges they have solve and are yet to overcome. Following lunch, the attendees will then be given ~1 hour to try out the different implementations and then break out into engineering-focussed sessions (topics to be decided during lunch on first day) for the rest of the afternoon.

| Time | Description |
|------|------|
| 08:30 — 09:00 | Coffee/light breakfast|
| 09:00 — 09:30 | Welcome/introductions/setting the stage (Arfon Smith & other organizers) |
| 09:30 — 10:30 | **Platform overviews:** 20 mins per implementer |
| 10:30 — 11:00 | Coffee |
| 11:00 — 12:00 | **Platform overviews continued:** 20 mins per implementer |
| 12:00 — 13:00 | Lunch, breakout session planning (at whiteboards) |
| 13:00 — 14:00 | Hands-on sessions with different tools |
| 14:00 — 15:00 | Breakout engineering session (i) (three separate rooms) |
| 15:00 — 15:30 | Coffee/snacks |
| 15:30 — 17:00 | Breakout engineering session (ii) (three separate rooms) |

**Platform overview** talks given by SciServer (Mike Rippen/Gerard Lemson), NOAO Datalab (Knut Olsen), NDS (Kenton Guadron McHenry), LSST (Frossie Economou), STScI (Christian Mesh), WholeTale (Kacper Kowalik), DES (Matias Carrasco-Kind). For each ‘platform overview’ talk we ask each implementer to cover the following points:

- A broad overview of what they’re building
- Who they’re building for (i.e. common use cases they anticipate supporting)
- Core technologies being used
- Key problems they’ve solved, key problems they still have

### Day 2 (27 February, 2018)

The second day is about focussing discussion on a number of key areas, with talks from a small number of individuals designed to stimulate discussion and then significant time devoted to working on technical solutions later in the day. For each 30 minute session the plan is to have a mix of presented content with ample time for questions.

| Time | Description |
|------|------|
| 08:30 — 09:00 | Coffee/light breakfast |
| 09:00 — 09:45 | **Interoperability & User Experience:** Short talks & discussion about interoperability and user experience |

**Interoperability suggested speakers/topics:**

- IVOA vs client libraries - Tom Donaldson & Brian Major
- Authorization/Authentication - Gregory Dubois-Felsmann/Frossie Economou?
- VODML - Gerard Lemson
- Authetication & Authorization in SciServer - Speaker TBD (SciServer)
- SciScript: client libraries for accessing SciServer REST APIs - Manuchehr Taghizadeh Popp (SciServer)
- Shared containers - Arfon Smith
- Mike Fitzpatrick (NOAO)

| Time | Description |
|-----|-----|
| 09:45 — 10:15 | **Managing users:**( Quotas, collaboration, training, user support| 

**Managing users suggested speakers:** Someone from SciServer, Datalab, NDS? (basically anyone _with_ users).

- Robert Nikutta (NOAO)
- SciServer's resource access control management solution - Jai Won Kim (SciServer)
- National Data Service?

| Time | Description |
|------|------|
| 10:15 — 10:45 | Coffee |
| 10:45 — 11:30 | Storage, file systems, data access: Short talks & discussion about these topics|

**Storage, file systems, data access suggested speakers & topics:**

- LSST's Butler - Jim Bosch
- Building user-workspaces on AWS - Christian Mesh (STScI)
- National Data Service?
- SciServer Compute as a containerized solution - Dmitry Medvedev (SciServer)
- Strategy and infrastructure for user file storage in SciServer - Joseph Booker (SciServer)

| Time | Description |
|------|------|
| 11:30 — 12:00 | Data models, pipelines, ORMs: How to represent scientific analyses in science platforms |

**Suggested speakers & topics:**
- LSST’s pipeline - Robert Lupton
- objcat - Erik Tollerud
- Batch processing with LSST – Frossie Economou / Gregory Dubois-Felsmann
- Batch processing in SciServer - Manuchehr Taghizadeh Popp (SciServer)

| Time | Description |
|------|------|
| 12:00 — 13:00 | Lunch, breakout session planning (at whiteboards) |
| 13:00 — 14:00 | Breakout engineering sessions (i) |
| 14:00 — 15:00 | Breakout engineering sessions (ii) |
| 15:00 — 15:30 | Coffee/snacks |
| 15:30 — 16:30 | Breakout engineering sessions (iii) |
| 16:30 — 17:00 | Report back on progress during breakout sessions. |

### Day 3 (28 February, 2018)

| Time | Description |
|------|------|
| 08:30 — 09:00 | Coffee/light breakfast |
| 09:00 — 10:00 | Report out on progress made on key topic areas over last two days |
| 10:00 — 10:30 | Sustainability, long term support |
| 10:30 — 11:00 | Coffee/snacks |
| 11:00 — 11:30 | Community contributions: Role of open source and wider community collaboration |
| 11:30 — 12:00 | Looking to the future: What’s next? Decadal, SnowPAC, future funding opportunities |
| 12:00 | Close |

**Possible speakers/topics**

- Hosting science data and software - Gerard Lemson (SciServer)

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
