# FAIR-RNA Manifesto

Version: 0.1.0 (first draft)

## Preamble

* CONSIDERING that we are a scientific community brought together from a wide
  variety of fields by a shared curiosity for RNA biology.

* CONSIDERING that every scientific endeavour is limited by its own rigour and
  thoroughness.

* CONSIDERING that the means of our science are diverse, complex and quickly
  evolving.

* CONSIDERING that computational approaches are now an integrative part of the
  RNA scientist toolkit.

* CONSIDERING that explicitly stating expectations helps create a more
  inclusive community and promote discussions of said expectations.

* CONSIDERING that SOFTWARE DEVELOPER, USER and PUBLISHER all have a
  responsibility towards ensuring the well-being of computational
  methodologies.

* We present here the FAIR-RNA Manifesto, devising guidelines for all actors of
  our community, in order to promote a FAIR, Open and rigorous scientific
  environment.

## Manifesto

> Software in this context refers to tools, packages and workflows for
> biological data analysis. While many statements are likely generally
> applicable to scientific software, or perhaps Open Source Software in
> general, they were composed by developers and users in the field of RNA
> research and with the specific state of software development in this domain
> in mind.

### For software developers

> The following guidelines are written from the perspective of code owners,
> i.e., the individuals or groups who are responsible for the maintenance of a
> Software. External contributors should follow the recommendations as well,
> if applicable, and help code owners comply with them.

#### Community involvement

* **Develop Free and Open Source Software under an appropriate license.**
  TODO: ANNO

* **Comply with license terms of any dependencies.**
  TODO: ANNO

* **Use Social Coding platforms to publicly host your codebase.**
  Apart from making the codebase available to users and potential contributors,
  Social Coding platforms typically offer useful tooling that helps developers
  to comply with the guidelines described here, such as support for version
  control software, project management functionalities (e.g., issue tracker,
  project boards), or integrated solutions for automated testing, code
  integration and code review. They are particularly well suited for
  collaborative development.

* **Describe how others can contribute to the development of your Software.**
  In order to encourage developers to contribute to existing Software instead
  of starting the development of a new related project, it is important that
  code owners provide guidelines on how external developers can meaningfully
  and productively contribute to development and decision making. Clearly and
  concisely describing existing requirements for proposed code changes to be
  merged into the codebase (e.g., adherence with a certain coding style,
  documentation updates, unit tests) will lower the entry barrier for potential
  contributors to engage with a software project.

* **Provide, comply with and enforce a welcoming code of conduct.**
  Research and developer communities usually thrive when different viewpoints
  are heard. Adding a code of conduct to your project may help make your team
  feel welcome and encourage an atmosphere of mutual respect between all
  contributors. Make sure to clearly outline steps to be taken if the code is
  violated.

* **Adopt a code review scheme.**
  Having one or more people review code that was proposed to be merged into the
  codebase strongly reduces the chance of introducing bugs. It is also a great
  way of learning to read code, finding out about new tipps and tricks, gaining
  confidence in your coding skills and team-building.

* **Provide clear governance information.**
  TODO: ANNO

#### Developing

* **Adopt a clear versioning scheme.**
  We recommend [semantic versioning](https://semver.org/) to make the evolution
  of your Software easily comprehensible to the community and avoid the descend
  into “dependency hell”.

* **Use version-control software to manage your codebase.**
  Version-control tooling helps you to collaborate with other developers and
  ensures provenance tracking of contributions. Moreover it helps you keep
  track of your development and enables you to restore your codebase to a
  former state, in case your code gets corrupted. When you publish your
  Software, version control is crucial for reproducibility, reusability and
  proper citation of your work.

* **Keep your codebase simple yet explicit.**
  Adhering to community standards for good coding practices will greatly
  increase the maintainability of your Software. Keep in mind to create modular
  code and comment extensively to enable yourself and others to use your
  Software.

* **Limit the scope of your Software.**
  Write small tools that perform one task well and refrain from creating a
  “God tool”. Maintainability is one of the core principles of FAIR-RNA, and it
  quickly becomes impossible when your codebase is growing and diversifying too
  much.

* **Implement intuitive programmable and extensible APIs for your Software.**
  Ensure modularity of your Software by precisely defining in- and outputs, and
  any adjustable parameters. To maximise reusability, do not "hardcode"
  parameters.

* **Use standardized file formats wherever possible.**
  Standardized file formats are a prerequisite for modularity and reusability,
  and thus sustainable software engineering. Consult
  [Edam](http://edamontology.org) for an ontology of formats common in your
  research community.

* **Provide informative log, debug and error messages.**
  Catch any errors early and safe time in development and frustration upon
  using your Software. Do not allow any ambiguous inputs but instead tailor
  your error messages and logs to create a convenient and trustworthy user
  experience.

* **Use workflow languages to connect individual processing steps.**
  In order to create reusable software, the sequence of individual steps has to
  be reproducible. Instead of writing custom solutions, use an existing
  well-maintained workflow language/engine that meets FAIR-RNA guidelines with
  respect to modularity, reusability, interoperability, maintainability,
  reproducibility and community involvement/usage.

* **Document your Software and keep documentation up-to-date.**
  Describe in detail how your Software can be used. Aim for a level of
  description that enables users with basic programming knowledge to run your
  Software. Comment critical portions of your code. Keep in mind that a user,
  your successor, or you yourself in the future will have difficulties in
  figuring out the rationale underlying tricky bits of code. Refrain from
  overcommenting as it bears the risk of comments and code diverging. The code
  remains the ultimate source of truth!

* **Continuously test your Software and ship your tests.**
  Ensure consistency of results produced by, and stable performance of your
  Software by performing regular integration tests. Provide tests for users to
  verify installation success and familiarize with your Software.

#### Building, packaging & publishing

* **Provide a simple build mechanism for your Software and document it.**
  Package management systems can help developers in ensuring that their
  software and dependencies will be properly installed and set up. To
  facilitate interoperability packaging of Software, ideally with all
  dependencies, is required. We strongly recommend containerization, as this
  will automatically enable Software for the cloud and is a means for packaging
  Software irrespective of programming languages and operating systems.

* **Automate building and publishing and adopt a fast release cycle.**
  Containerization as described above will also facilitate continuous
  integration and deployment (CI/CD) approaches, which are crucial to the
  robust growth of your Software. By committing to a CI/CD solution, changes
  you make to your code can automatically be built, tested and, if all tests
  were successful, deployed. Like this, new features or bugfixes can be
  included easily and safely, without any downtime for your Software. You
  remain flexible and can quickly adapt and react to current developments and
  user requests.

* **Obtain a citable identifier for your Software.**
  Distributing your Software with a persistent citable identifier establishes
  it as a tool of scholarly interest. This identifier should be easily
  findable, and should interconnect the relevant items, such as Software,
  publication(s), author(s). This identifier can also track the usage of the
  Software in the literature, enabling Software meta-analysis and oversight.

* **Publish your Software in one or more suitable repositories.**
  Using centralized and well established in-domain repositories facilitates the
  usage of the Software by the community.

* **Provide FAIR metadata relevant for your Software.**
  Consult the
  [FAIR principles for research software](https://content.iospress.com/articles/data-science/ds190026)
  to gain some insight in which metadata might be relevant to your Software.
  There are several ongoing initiatives like
  [Bioschemas](https://bioschemas.org/) that are developing ontologies for
  human and machine readable metadata. As a minimum requirement we recommend
  to include source code location, contributors, license, references, how to
  cite the software and a concise description of what the Software
  does.

* **Ensure all contributors are given fair credit for their work.**
  Adhering to this fundamental principle is the first step towards a FAIR
  research environment.

* **Let your Software die gracefully.**
  When maintainability is not feasible, or not necessary because the Software
  has been superseded by another one, it is necessary to deprecate the
  Software. It still should be available for benchmarking or reproducibility
  studies, but new users should be discouraged from engaging with it.

### For software users

> Follow these guidelines if you are using Software as is, without making
> any modifications.

* **Prefer Software that complies with FAIR-RNA guidelines.**
  By using, citing and recommending compliant Software you actively participate
  in creating a FAIRer world.

* **Comply with license terms of Software.**
  TODO: ANNO

* **Cite all used Software.**
  Give credit where credit is due and enable other researchers to fully
  comprehend your approach.

* **Report used versions of all Software.**
  In order to ensure reproducibility of your work, it is crucial that you
  supply the correct version of the Software used. Published Software may
  develop rapidly, and newer versions might not produce the same results, nor
  support the same API that was the foundation of your work.

* **List all non-default parameters that were used and justify their choice.**
  Help other people understand your rationale and ensure reproducibility of
  your work. Enable the community to adapt your work to their needs and
  contribute to the global creation of knowledge.

* **Report details of your runtime environment.**
  Using workflow management software that wraps environment definition,
  Software installation and usage helps provide all crucial information to
  recreate the study.

### For software publishers

> Software publishers include code hosting services, specialized repositories
> for tools, packages and workflows, and scientific journals.

* **Comply with [FAIR](https://www.go-fair.org/fair-principles/) Principles.**
  Ensure that the published Software is findable, interoperable and reusable by
  encouraging the inclusion of extensive human and machine readable metadata.
  Make the Software accessible by implementing standardized communication
  protocols.

* **Request that Software comply with FAIR-RNA guidelines.**
  By encouraging adherence to FAIR-RNA guidelines you will ultimately increase
  your own traffic, as the Software published in your domain will be more easy
  to (re)use and demand and citations increase.

* **Provide infrastructure to support FAIR-RNA guidelines.**
  TODO: ANNO
