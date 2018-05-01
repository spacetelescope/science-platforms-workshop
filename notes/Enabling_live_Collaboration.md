Science platforms/Server Side Analytics workshop
STScI
Feb 27, 2018

# Enabling (live) collaboration

## Short link: http://bit.ly/spssa18-livecollab 

* This session is about live collaborating on live collaborating
* Collaboratory? (by google)
  * It’s maybe deprecated because Google deprecated the relevant API
	* may be resurrected: https://research.google.com/colaboratory 
* Do we actually *want* to do live collaboration?
  * It could be an end-run around software engineering
    * Notebooks make it hard to do the good stuff
    * But that’s an eng perspective - nbs are more about “data exploration”
    * If science platforms actually work, that might *become* the way people make their code
    * But some stuff maybe isn’t meant for “integrated” workflow
    * Regardless, there should be a way to deliver nb as “software”.  Whether live is bad or not, it needs to be testable/engineerable
      * This *is* possible, but it’s hard to do Pull Requests
    * What about education?
* LSST is going to … SOMEONE FROM LSST SHOULD ALSO HELP TAKE THE NOTES
* Are there other “google docs for notebooks”?
  * Swan https://swan.web.cern.ch/ may be working on live-collab?
  * Jupyter team may be “digesting” google’s stuff
  * But probably no one today has implemented the “google docs for notebooks”
* Should astronomers write it
  * No
* What about “hacks”
  * Discussion of Erik/Josh’s nb trick
    * May not work in lab?  Might be intentional.  Jupyter folks want notebooks to be “stateful”
    * Jupyter details...
* LSST is building a Jupyterlab extension to do ds9-y things
  * Users want the “ds9 window” to be off to the side even as the notebook scrolls
* Maybe it’s good enough to have the “collaboration” be just the fancy widget-y things, but not the notebook itself?
* Another “easier” version is to have one writer but multiple viewers (“pass the ball”)
  * May be easier in the current scheme?
  * Avoids a lot of the concerns of how to “sync” multiple users at once
* What about Zeppelin? (https://zeppelin.apache.org/) 
  * Not quite as Python-supporting?  But maybe it’s better now?
  * Claim to want to support the collaborative stuff
* Astronomers are very technologically conservative, so hard to get them to use new tools
  * User bases is already using Jupyter, which is why LSST is adopting it
  * But it’s pretty easy for “science platforms” to support this stuff
* Erik says some rabid “open science” things that kind of derail the conversation
  * But maybe it’s a good idea to provide Google Drive style “view link” to make this fairly straightforward?
* Notebooks are “ordered” with a causal flow, so maybe the “collaboration” is bad
  * But still compatible with the “one driver” mode
  * Different from a “screen sharing” collaboration because you can’t scroll out of view
* Frossie repeats the concern about diffs in PRs for nbs - it makes it impossible to do a proper eng workflow
  * But it should be straightforward if someone on github gets behind it?
