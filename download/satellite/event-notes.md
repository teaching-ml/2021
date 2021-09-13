# Teach ML Satellite event Sep 8, 2021

## House Keeping

- **This event is subject to the [ECMLPKDD2021 code of conduct](https://2021.ecmlpkdd.org/?page_id=2082)!** Please be supportive in your communication. If you feel you witness violations or are subject thereof, please report this to the organizers privately.

- This event is recorded and will be published on youtube! Please disable your camera, in case you do not want to be filmed.

- Please mute yourself while you are not talking. 

# Agenda

The full agenda is also documented on our workshop website:
https://teaching-ml.github.io/2021/#preface-satellite-event---september-8-2021

Video conference details: https://us06web.zoom.us/j/89839487704?pwd=QXp3MWc4WVNTRFdBeldhRWVBU0RwUT09

## Katherine Kinnaird + Peter Steinbach: Welcome

### Notes or Questions

## Cornelia Gamst: Demo of "AI Campus - the learning platform for artificial intelligence"

Everybody (well, almost) wants to learn Machine Learning, or Data Science these days. The big online learning platforms already offer a wide variety of options, differing in level, length, depth and also learning formats. But somehow in Germany there still seems to be a missing piece. "AI Campus" wants to fill that gap with specialized courses and learning nuggets for a broad target group: from in depth courses for domain experts to learning nuggets offering a basic understanding of what's behind AI and machine learning for the general public.

In this workshop, we will give a brief demo of learning formats available on AI Campus, discuss our general curriculum framework and we can take a closer look at how we do things in specific courses that are of interest to the audience of the workshop.

### Notes or Questions

* What are your wishes for a platform like AI Campus?
* Which content or what feature would make you want to use AI Campus?


- LTI standard (Learning Tools Interoperability (LTI) Assignment and Grade Services Specification): https://www.imsglobal.org/spec/lti-ags/v2p0

- Question: MOOCs reportedly have a high dropout rate. Can you confirm and falsify this for AI campus based on your learner statistics?
    - launched one year ago
    - user numbers are comparably low (if compared to other international platforms) so persistance rate is hard to trust
    - in the context of university setting, persistance rate is higher as students need the final certificate
- Question: How many learners have been enlisted? How many learners can you enlist?
    - depends on the course
    - 6k learners on the platform, 200-2000 enrollments for each course
- Question: How many software engineers are working on/for the AI Campus website?
    - hard to get funding for RSEs or other human resources to support the online infrastructure

- Question: if the lessons are based on jupyter notebooks, new languages entail a "clone" of the jupyter notebook, right?
    - translation is demanding (especially with videos)
    - courses offered either in German or English
    - carpentries are prototyping with dictionaries used within websites (which are then translated)
        - blog post on more human-driven translation: https://carpentries.org/blog/2019/01/python-ecology-es/
        - issue propsing automatic translation via tokens to manage it with verisoning: https://github.com/carpentries/lesson-infrastructure/issues/24
        - example rendered site: https://carpentries-i18n.github.io/git-novice/ 
        - SB comment: using this scheme with notebook files would probably be well served by something like [jupytext](https://jupytext.readthedocs.io/en/latest/) as well to maintian the notebooks as plain text instead of json (.ipynb is a json file)
    - https://programminghistorian.org/en/translator-guidelines 
        - challenge here is to keep translations in synch with the `main` content
- Question: Do you also plan on offering lessons for school students?
    - maybe: focus area of AI campus are the teachers (rather than high school students)
    - some courses contain material/exercises that educators can reuse
- Question: Do you consider having learning paths or a similar idea to connect different courses or topics?
    - yes! this was planned from the beginning but is limited by RSE resources 
    - micro degrees may be helpful here (maybe coming soon)
    - recommender systems on the design board (which help learners to suggest )
     
**Please get in touch**, if you have further feedback or are interested in AI Campus: 
cornelia.gamst@ki-campus.org 


## Sorelle Friedler: Embedding Ethics in Data Structures Classes

Fairness in machine learning, or more broadly AI Ethics, has become a hot
topic in research over the past 5 years and these topics are increasingly
being incorporated into the machine learning and AI curriculum. In this
talk, I'll argue that we can best prepare our students to participate in
these conversations and build better machine learning systems by
introducing them to ethical ideas early in the curriculum. Data Structures,
generally taught in the second semester of a college computer science
curriculum, is an early and required class where students learn to think of
themselves as problem solvers. Integrating data-driven real world projects
and associated ethical concerns into data structures teaches students the
background they'll need to build better ML. I'll discuss projects
integrating racial equity concerns and environmental impact into the data
structures curriculum.

### Notes or Questions

- https://responsibleproblemsolving.github.io/ 
- ProPublica article [Machine Bias](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing) All data from this article has been released
- https://codecarbon.io/ 
- [Teaching Responsible Computing Playbook](https://foundation.mozilla.org/en/what-we-fund/awards/teaching-responsible-computing-playbook/)

- Question: when discussing the effects of data on the inference being made (e.g. with respect to the risk of people being arrested again) to what level are students exposed to aspects of experimental design (i.e. with respect to confirmation bias or including observables/parameters that help falsify the hypothesis etc)?
    - Incorporating this into a statistics course (instead of a CS course) would be very different. In this CS context, experimental design is not directly taught. Students who have that experience will bring this in. (Note that Haverford is a liberal arts college. Students have a wide variety of experiences). Perhaps the intersection of experimental design and computing would be better for a data science course. 
    - Comment from Peter - Perhaps it's good that experimental design is not directly included. Perhaps you can just direct students to explore this on their own. 

- Question: this is a collaborative effort - was it a challenge to find collaborators?
    - between institutions collaboration: based on common interest coming from a background trying to understand algorithms
    - collaboration within the institution: Many people interested in these ideas, and also many people teaching this course as well. Happened organically to some degree. Passing materials between colleagues helped develop better materials where context was missing from the original materials

- Comment: Great content - the idea of wiring the ethical aspect into a practical assignment is really amazing. We made the experience and got the feedback from the students that a theoritical treatment is sometimes relatively boring, especially in the context of a machine learning class.
- 


## Alicia Johnson: Rethinking the dreaded textbook: taking inspiration from the inclusive, ethical, and active machine learning classroom

As machine learning educators, we’re trained to translate and
weave developing “best practices” into our classrooms. For example, we
might aim to create inclusive courses which center data ethics while
promoting active learning. Especially since these same ends aren’t always
embedded in our classroom resources (eg: textbooks), pulling this off can
require some patchwork and wizardry. In this talk, we’ll discuss Bayes
Rules! An Introduction to Bayesian Modeling with R (Johnson, Ott, &
Dogucu), our attempt at: (1) supporting educators in their implementation
of inclusive, ethical, and active learning practices; and (2) reflecting
that these goals are critical to the entire machine learning workflow, not
just the classroom; all while (3) being ourselves.

### Notes or Questions

- "Bayes Rules!" book: https://www.bayesrulesbook.com/
- Data Feminism book: https://data-feminism.mitpress.mit.edu/

- Question: I wonder if alt text explanations of images would help non-impaired readers too? For example to cognitively reinforce the concepts conveyed if the alt text repeats a concept in a different way.

- Question: when writing the book, did you keep reader personas at your side to remind yourself for whom you are writing this text? If so, how did you come about with those personas.

## Katherine Kinnaird + Peter Steinbach: Homework and Farewell

Survey to find out what our community is interested in discussing next week:
https://bit.ly/teachingML-2021 