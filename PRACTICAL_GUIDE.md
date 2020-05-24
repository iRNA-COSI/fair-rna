# FAIR-RNA Practical Guide

FAIR-RNA Practical Guide

The following guide accompanies the FAIR-RNA manifesto, in order to provide additional inspiration on how to abide by the recommendations stated in the manifesto. It is, by nature, by no means comprehensive, nor are all cited resources necessarily FAIR-RNA compliant. Instead, the practical guide is meant to serve as an entry point for USERS, DEVELOPERS and PUBLISHERS to familiarize themselves with the concepts of FAIR-RNA. We therefore collected a wide range of popular resources that introduce, explain, implement or provide aspects of these concepts stated in the manifesto. Note that we do not endorse any of the resources and, in particular, do not wish to recommend them over others, which may not be listed here. With growing community engagement and dynamics, we hope to extend the guide in the future to highlight FAIR-RNA compliant Software and foster the development of the former.

## For DEVELOPERS

### Develop Free and Open Source Software under an appropriate license

Developing software with freely available source code is essential for providing usability and transparency to your intended end-users. The Open Source Initiative and Free Software Foundation are non-profit groups dedicated to promoting free-use software and are good resources for deciding on an open source license.

**Resources:**

* Choosing a license: <https://choosealicense.com/>
* Open Source Initiative: <https://opensource.org/>
* Free Software Foundation: <https://www.fsf.org/>

### Comply with license terms of any dependencies

TODO

**Resources:** TODO

### Use Social Coding platforms to publicly host your codebase

Social coding refers to platforms that promote community engagement and support among developers. This puts a focus on open, collaborative development projects.

**Resources:**

* Getting started with social coding on GitHub: <https://opentechschool.github.io/social-coding/>
* Why to use social coding platforms: <https://www.ibm.com/garage/method/practices/culture/practice_social_coding/>
* BitBucket: <https://bitbucket.org/>
* GitHub: <https://github.com/>
* GitLab: <https://about.gitlab.com/>
* Google Code: <https://code.google.com/>

### Describe how others can contribute to the development of your Software

TODO

**Resources:** TODO

### Provide, comply with and enforce a welcoming code of conduct

TODO

**Resources:** TODO

### Adopt a code review scheme

TODO

**Resources:** TODO

### Provide clear governance information

TODO

**Resources:** TODO

### Adopt a clear versioning scheme

Version control schema are a structured way in which developers collaborating on a project can coordinate and track changes to the software. This can make large-scale project development much more manageable. Semantic versioning is a popular versioning schema in which a software version is broken into three aspects: patch, minor, and major updates. Patches are small changes and bug fixes which do not affect the API. Minor updates modify or add functionality to the software while retaining backwards compatibility. Major updates represent large changes which affect the API in a non-backwards compatible way. This versioning is often formatted as X.Y.Z, where X corresponds to the major update version, Y corresponds to the minor updates within the major update version, and Z corresponds to patches within the minor update version.

**Resources:**

* Semantic Versioning: <https://semver.org/>
* Tutorial for semantic versioning with Git tags: <https://travishorn.com/semantic-versioning-with-git-tags-1ef2d4aeede6>

### Use version-control software to manage your codebase

Version control software provides a structured framework for developers to manage versions, test and debug changes, and push updates to projects. These tools are invaluable for coordinating collaborative projects which feature regular updates and are intended for long-term sustainability.

**Resources:**

* Tutorial for version control using Git: <https://ourcodingclub.github.io/tutorials/git/#version>
* BitKeeper: <http://www.bitkeeper.org/>
* Git: <https://git-scm.com/>
* Mercurial: <https://www.mercurial-scm.org/>

### Keep your codebase simple yet explicit

**Resources:**

* Guide to PEP8 style guide for Python: <https://www.python.org/dev/peps/pep-0008/>
* Primer to using modular programming to reduce code complexity: <https://www.toptal.com/software/creating-modular-code-with-no-dependencies>
* Primer to modular and maintainable code when developing an application: <http://singlepageappbook.com/maintainability1.html>
* Primer to single responsibility principle: <https://code.tutsplus.com/tutorials/solid-part-1-the-single-responsibility-principle--net-36074>

### Limit the scope of your Software

Smaller, focused tools are more intuitive to users and maintainable for developers. By focusing development on creating a powerful tool that performs a specific task, developers protect users from becoming overwhelmed when interacting with it and protect themselves from being inundated with blending many functions into a single product. Going beyond the scope of the intended functionality to add additional, niche-case features can seem like a benefit at first, but can easily spiral into an unmanageable tangle of additions that are not needed by the users.

**Resources:**

* Primer to developing maintainable software: <https://software.ac.uk/resources/guides/developing-maintainable-software>

### Implement intuitive programmable and extensible APIs for your Software

An API (Application Programing Interface) defines how a user (or other programs) can interact with your software. The API defines a set of functions and calls that your software is able to interpret and respond to, which provides end-users a way to use the software. Creating a robust API can have a large impact on how practical the users find your software to be.

**Resources:**

* Primer on API development: <https://appinventiv.com/blog/complete-guide-to-api-development/>
* Considerations for better API design: <https://medium.com/better-practices/design-apis-like-you-design-user-experience-a7adeb2ee90f>

### Use standardized file formats wherever possible

When developing software, adhering to standard formats makes interacting with the software and interpreting results more intuitive. In addition, keeping to standard formats for input and output makes software more easily integrated into analysis pipelines and more intuitive to users.

**Resources:**

* Descriptions (non-exhaustive) for commonly used file formats in bioinformatics: <https://genome.ucsc.edu/FAQ/FAQformat.html>
* Comprehensive ontology of data types, formats, and operations commonly used in bioinformatics: <http://edamontology.org/>

### Provide informative log, debug and error messages

Logs are records detailing what is going on with your software in real time. Proper logging throughout the development process can save the developer and user a lot of headache down the road. Informative error logs assist developers in debugging and users understand why a task has failed.

**Resources:**

* Tutorial on logging with Python: <https://docs.python.org/3/howto/logging.html>
* Best practices for logging during development: <https://www.scalyr.com/blog/the-10-commandments-of-logging/>

### Use workflow languages to connect individual processing steps

As the name suggests, workflow languages facilitate the creation of workflows, by allowing the developer to wire a sequence of processing steps (scripts or short commands) in the desired order. The workflow engine takes care of executing individual steps in the correct order and in the appropriate environment (locally or on high performance clusters). It furthermore provides extensive logging and provenance information, and ensures reproducibility of an analysis.

**Resources:**

* Snakemake: <https://snakemake.readthedocs.io/en/stable/>
* Common workflow language: <https://www.commonwl.org/>
* Nextflow: <https://www.nextflow.io/>
* Wdl: <https://openwdl.org/>
* Galaxy: <https://usegalaxy.org/>
* List of existing workflow systems (number of entries is good example why you shouldn’t try to reinvent the wheel): <https://github.com/common-workflow-language/common-workflow-language/wiki/Existing-Workflow-systems>

### Document your Software and keep documentation up-to-date

When you are writing code, you are doing it for two audiences: your developers (including your future self) and your users. Both audiences should be able to understand what you want them to do, which makes it important to describe your Software on different levels. While documentation explains the structure of the project, how to install it and how and why it works, commenting enables developers (you!!) to understand non-trivial choices in your coding.

**Resources:**

* Primer on project documentation: <https://github.com/writethedocs/www/blob/master/docs/guide/writing/beginners-guide-to-docs.rst>
* Primer on commenting: <https://www.freecodecamp.org/news/code-comments-the-good-the-bad-and-the-ugly-be9cc65fbf83/>
* Extensive Python how-to: <https://realpython.com/documenting-python-code/>

### Continuously test your Software and ship your tests

Robust test sets are an essential debugging tool for developers. The more rigorously a software is tested, the better equipped developers will be to identify and fix errors before they are encountered by users. As projects get larger and more collaborative, extensive testing, at both the unit and integration levels, becomes even more important. Unit testing ensures that individual, modular components of the software are working properly. Integration testing determines whether the individual modules of the software are able to work together cohesively. Maintaining large projects with many changing parts need regular testing to ensure that modifications in one place do not have unforeseen effects on itself or other parts of the project. In addition to helping developers, test sets can be useful to users in determining whether an installation was successful.

**Resources:**

* Primer on testing code in Python: <https://docs.python-guide.org/writing/tests/>
* Primer on writing testable code: <https://www.toptal.com/qa/how-to-write-testable-code-and-why-it-matters>
* Introduction to unit, integration, and functional testing: <https://www.softwaretestinghelp.com/the-difference-between-unit-integration-and-functional-testing/>

### Provide a simple build mechanism for your Software and document it

If you have installed let’s say more than 3 non-mainstream software programs in your life, you have probably come across dependency conflicts and incompatibilities with your operating system. You have most likely already spent hours of your life trying to get a particular program to run, failed, and consequently didn’t use it and were not very eager to recommend it to a friend. In order to avoid this fate for your Software, make it as easy as possible for the user to install and run it. There are many efforts out there, that either provide package distribution for individual programming languages, or even allow language-agnostic management of packages and environments. Using containerization solutions is even more powerful, as you become platform independent and can thus reach a bigger audience.

**Resources:**

* Containerization (Docker primer): <https://www.docker.com/resources/what-container>
* Package, dependency and environment management (Conda): <https://docs.conda.io/en/latest/>
* R package repository (R-CRAN): <https://cran.r-project.org/>
* Python Package Index (PyPi): <https://pypi.org/>

### Automate building and publishing and adopt a fast release cycle

TODO

**Resources:** TODO

### Obtain a citable identifier for your Software

The most widely used identifier for research software is the digital object identifier (DOI), that is also used for scientific publications. DOI is a persistent unique number combination that can provide long-term links to data sets, articles and software. In order to obtain a DOI you need to use a service offered by a DOI Registration Agency (RA). There are suitable repositories that offer DOI registration as mentioned in the next section.

**Resources:**

* DOI system FAQs: <https://www.doi.org/faq.html>

### Publish your Software in one or more suitable repositories

In order for your software to become widely used it has to be published in a well known repository and accessible by the community. Data availability facilitates data validation, reproducibility, and ensures recognition for data producers, curators and authors. While social code development and sharing sites are invaluable assets in software development, they are not necessarily suited to archive software and provide sufficient metadata. However, in the case of Github, you do not have to create a new repository in order to publish. The links provided below explain how you can publish your github repository to make it citable.

**Resources:**

* Publish from Github to Zenodo: <https://guides.github.com/activities/citable-code/>
* Publish from Github to figshare: <https://figshare.com/blog/figshare_launches_revamped_GitHub_integration/243>

### Provide FAIR metadata relevant for your Software

TODO

**Resources:**

* Software Metadata tutorial: <https://softdev4research.github.io/4OSS-lesson/05-use-registry/index.html>
* Registry for bioinformatics software and databases: <https://bio.tools/>

### Ensure all contributors are given fair credit for their work

Within multidisciplinary teams, it becomes important to identify accountability through full disclosure of each participant’s contribution to the work. The extent of each participant’s relative contribution should be mutually agreed upon among the team members; one way is to numerically rank contributions with relative weightings to empirically outline the order of the authorship list. The discussion of who will receive credit and to what extent based on agreed upon responsibilities should be outlined in the earliest stages of a project.

**Resources:**

* <https://www.frontiersin.org/articles/10.3389/fpsyg.2011.00196/full>

### Let your Software die gracefully

TODO

**Resources:** TODO

### For USERS

### Prefer Software that complies with FAIR-RNA guidelines

Use of FAIR-RNA compliant software perpetuates a positive feedback loop that also gives credit to the developer team. By actively recommending and citing where credit is due, this builds momentum for more developers and researchers alike to join in a FAIRer world. The benefits of compliance; accessibility, reproducibility and interoperability to name a few, work best when we work towards an ecosystem of FAIR software from start to finish.

**Resources:**

* <https://www.nature.com/articles/sdata201618>

### Comply with license terms of Software

TODO

**Resources:** TODO

### Cite *all* used Software

From the Force11 recommendations (<https://peerj.com/articles/cs-86/>): “Software should be considered a legitimate and citable product of research. Software citations should be accorded the same importance in the scholarly record as citations of other research products, such as publications and data.”

**Resources:**

* How to cite software: <https://libguides.mit.edu/c.php?g=551454&p=3900280>

### Report used versions of all Software

TODO

**Resources:** TODO

### List all non-default parameters that were used and justify their choice

Specify how exactly you used the software. If you didn’t change any default settings, mention this as well to make transparent how you performed your analysis.

**Resources:** TODO

### Report details of your runtime environment

TODO

**Resources:** TODO

### For software publishers

### Comply with FAIR Principles as applicable for data providers

TODO

**Resources:**

* GO-FAIR: <https://www.go-fair.org/go-fair-initiative/>
* Internet of FAIR Data & Services: <https://www.go-fair.org/resources/internet-fair-data-services/>

### Request that Software comply with FAIR-RNA guidelines

TODO

**Resources:** TODO

### Provide infrastructure to support FAIR-RNA guidelines

TODO

**Resources:** TODO
