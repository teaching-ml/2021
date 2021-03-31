# ECML2021 teachML workshop

This folder tries to serve as a central hub to draft for a ECML2021 workshop submission on teaching methods for ML. 

See [this link](https://gitlab.com/psteinb/icml2020-teachml-workshop/-/jobs/artifacts/master/browse?job=compile_pdf) to obtain the latest pdf version of this draft. A zip file containing this pdf is available [here](https://gitlab.com/psteinb/icml2020-teachml-workshop/-/jobs/artifacts/master/browse?job=compile_pdf).

## How to help

If this proposal is accepted, we need some help potentially. If you'd like to become a co-organizer, please submit a merge request which adds yourself to [99-authors_supporters.md](99-authors_supporters.md). 

If you'd like to support our cause and indicate your will to either attend or to submit something, please do so by adding your name to the supporters section of [99-authors_supporters.md](99-authors_supporters.md) or create an issue indicating your support.

Besides any of the above, constructive feedback is highly welcome. Please open an issue for this.

## What We need to submit

According to the [ECML2021 Workshop page](https://2021.ecmlpkdd.org/?page_id=1603), the submission document should include:

> Workshop proposals should contain the necessary information for the workshop chairs and reviewers to judge the importance, quality, and community interest in the proposed topic (a minimum of 20-30 expected participants is required). Each workshop should have two or more designated organisers and a program. When proposing a workshop, please provide (at least) the following information:
> 
> * A brief description of the specific topics that the workshop will address, the reasons why the workshop is of interest, the main research areas involved, and what the workshop will add to the conference.
> * Contact information of the workshop chairs, their competence in the proposed topic(s), and previous experience in chairing scientific events. 
> * A tentative list of Program Committee members and potential invited speakers.
> * A draft of the Call for Papers, including information on accepted formats (e.g., regular papers, extended abstracts, oral-only presentations of relevant recently published or submitted contributions, etc.) and expected format of the workshop (e.g., invited talks, presentations, poster sessions, panel discussions, challenge sessions, or other ideas for ensuring an interactive atmosphere). In the case of a combined tutorial-workshop, please clearly indicate the format.
> * Any special requirements regarding logistics (e.g., poster stands, audio equipment), if applicable.
> * An estimate of the number of expected submissions, and an estimate of the number of expected workshop participants at the conference. Proof of interest from the community will be of added value to the proposal.
> * If you are making a proposal for a tutorial+workshop event, we kindly ask you to write a single proposal that covers both. In addition, the links should be clearly described and the proposal should be submitted to the workshop and tutorial chairs (select ‘Workshop and Tutorial’ as the topic on Easychair). For tutorial guidelines, please see the separate Call For Tutorial Proposals.

Regarding the format, the following is expected:

> Proposals should be two pages long in single column A4 or letter format, with font size 11 or greater, excluding organiser contact details/CVs and bibliographic references.

The easychair submission page in addition asks for a title and an abstract. I hope that will be in the line with "A brief description of the topics to be covered ..." from above.

## How to build

In order to keep the technological overhead low, I opted for using markdown (rendered by [pandoc](https://pandoc.org) using latex in the background) as the central tool to document the draft and a GNU Makefile to handle the build. The build assumes a *NIX like OS (Linux, macOS and Linux Subsystem for Win10).

``` shell
$ make 
```

