# ECML2020 teachML workshop

This repo tries to serve as a central hub to draft for a ECML2020 workshop submission on teaching methods for ML. 

See [this link](https://gitlab.com/psteinb/icml2020-teachml-workshop/-/jobs/artifacts/master/browse?job=compile_pdf) to obtain the latest pdf version of this draft. A zip file containing this pdf is available [here](https://gitlab.com/psteinb/icml2020-teachml-workshop/-/jobs/artifacts/master/browse?job=compile_pdf).

## How to help

If this proposal is accepted, we need some help potentially. If you'd like to become a co-organizer, please submit a merge request which adds yourself to [99-authors_supporters.md](99-authors_supporters.md). 

If you'd like to support our cause and indicate your will to either attend or to submit something, please do so by adding your name to the supporters section of [99-authors_supporters.md](99-authors_supporters.md) or create an issue indicating your support.

Besides any of the above, constructive feedback is highly welcome. Please open an issue for this.

## What We need to submit

According to the [ECML2020 Workshop page](https://icml.cc/Conferences/2020/CallForWorkshops), the submission document should include:

> * Workshop title
> * A brief description of the topics to be covered, and an explanation as to why the workshop will appeal to ECML audiences
> * A short description and rough timetable of the planned activities (talks, posters, panels)
> * List of invited speakers, specifying who is confirmed and who is unconfirmed.
> * A description of the history of the workshop (if it previously took place then when/where)
> * Similar past and current events at ECML and NeurIPS in the last 1-2 years, even if not organised by the present workshop organisers. New workshops are welcome to build on prior workshops, if a good case is made; completely original workshops are also welcome.
> * A list of organizers with email addresses, web page URLs, pointers to Google Scholar or other similar citation service pages, and a one-paragraph bio for each organizer, describing research expertise, and previous experience organizing scientific meetings.

Regarding the format, the following is expected:

> Proposals should be two pages long in single column A4 or letter format, with font size 11 or greater, excluding organiser contact details/CVs and bibliographic references.

The easychair submission page in addition asks for a title and an abstract. I hope that will be in the line with "A brief description of the topics to be covered ..." from above.

## How to build

In order to keep the technological overhead low, I opted for using markdown (rendered by [pandoc](https://pandoc.org) using latex in the background) as the central tool to document the draft and a GNU Makefile to handle the build. The build assumes a *NIX like OS (Linux, macOS and Linux Subsystem for Win10).

``` shell
$ make 
```

