# The FAIR-RNA Manifesto

Version: 0.3.0

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

* CONSIDERING that DEVELOPER, USER and PUBLISHER all have a responsibility
  towards ensuring the well-being of computational methodologies.

* We present here the FAIR-RNA Manifesto, devising guidelines for all actors of
  our community, in order to promote a FAIR, Open and rigorous scientific
  environment.

## Manifesto

> SOFTWARE in this context refers to tools, packages and workflows for
> biological data analysis. While many statements are likely generally
> applicable to scientific software, or perhaps Free and Open Source Software
> in general, they were composed by DEVELOPER and USER in the field of RNA
> research and with the specific state of software development in this domain
> in mind.

### For DEVELOPER

> The following guidelines are written from the perspective of code owners,
> i.e., the individuals or groups who are responsible for the maintenance of a
> SOFTWARE. External contributors should follow the recommendations as well,
> if applicable, and help code owners comply with them.

#### Community involvement

- [ ] **Develop Free and Open Source Software under an appropriate license.**  
  Free and Open Source Software (FOSS) has several advantages in particular for
  small teams and organizations as are often found in academia and the
  scientific software sector as a whole, including: FOSS involves the community
  in development and decision-making and is thus rested on a broader
  foundation/consensus, favoring adoption; it is inherently transparent and
  thus capable of improving reproducibility and facilitating rigorous reporting
  standards; it enables continuous code review and thus improves on the peer
  review process for scientific literature that is typically taking place only
  at or towards the end of a project; it allows for more flexible use of
  SOFTWARE, including in settings where funding is short.

- [ ] **Contribute to existing SOFTWARE instead of developing a similar one.**  
  While it may be tempting to start developing your own SOFTWARE to be in total
  control of all development decisions and share the credit for your work with
  less people, consider that it is wasteful to "reinvent the wheel" and not
  build on existing work. Also consider your potential USER who will have a
  hard time deciding between different software solutions. We thus recommend
  to search if there is already a similar SOFTWARE out there and try to
  dedicate your ideas and development time to that project instead. Try to
  encourage the code owners to consider abiding by the FAIR-RNA guidelines, if
  they do not already do so. If contributing to the existing SOFTWARE is not an
  option, but the SOFTWARE is publicly available FOSS, consider forking it,
  instead of starting an entirely new codebase.

- [ ] **Comply with the licensing terms of any dependencies.**  
  To avoid legal proceedings against you, comply with licensing terms of all
  dependencies at all times. Moreover, to maximize the use of your Free and
  Open Source Software, pick your dependencies carefully and be aware of how
  their licensing terms may affect the freedom of your own SOFTWARE or license.
  This is particularly important if potential dependencies adopt "unfree"
  and/or "viral" licenses.

- [ ] **Use Social Coding platforms to publicly host your codebase.**  
  Apart from making the codebase available to USER and potential contributors,
  Social Coding platforms are particularly well suited for collaborative
  development, as they typically offer useful tooling that helps DEVELOPER
  to comply with the guidelines described here, such as support for version
  control software, project management functionalities (e.g., issue tracker,
  project boards), or integrated solutions for automated testing, code
  integration and code review.

- [ ] **Describe how others can contribute to the development of your SOFTWARE.**  
  In order to encourage DEVELOPER to contribute to existing SOFTWARE instead
  of starting the development of a new related project, it is important that
  code owners provide guidelines on how external contributors can meaningfully
  and productively contribute to development and decision making. Clearly and
  concisely describing existing requirements for proposed code changes to be
  merged into the codebase (e.g., adherence with a certain coding style,
  documentation updates, unit tests) will lower the entry barrier for potential
  contributors to engage with a SOFTWARE project.

- [ ] **Provide, comply with and enforce a welcoming code of conduct.**  
  Research and development communities usually thrive when different viewpoints
  are heard. Adding a code of conduct to your project may help make your team
  members feel welcome and encourage an atmosphere of mutual respect between
  all contributors. Make sure the code clearly outlines how violations should
  be reported, which steps will be taken as a consequence and how potential
  conflicts of interest (e.g., if allegations of code violation are raised
  against yourself) are to be resolved.

- [ ] **Adopt a code review scheme.**  
  Having one or more people review code that was proposed to be merged into the
  codebase strongly reduces the chance of introducing bugs. It is also a great
  way of learning to read code, finding out about new tipps and tricks, gaining
  confidence in your coding skills and team-building.

- [ ] **Provide transparent governance information.**  
  Be mindful that external contributors give up control over a project if they
  decide to forego starting their own similar project and contribute to a
  project that is owned by you instead. If you value the contributions and
  visions of the community, make sure to transparently outline how decisions
  are made within your project and if and how external contributors can take
  part in that process. Whenever possible and reasonable, try to achieve a
  consensus among the major stakeholders, as this will not only increase
  your contributors' satisfaction but also likely increase community adoption
  of your SOFTWARE.

#### Developing

- [ ] **Adopt a clear versioning scheme.**  
  Versioning your SOFTWARE allows is a prerequesite for its USER to use it
  correctly and accurately report its use. It also facilitates the
  implementation of a transparent development and release cycle. We recommend
  [Semantic Versioning][semver] for its clarity and wide adoption. If using
  a custom versioning scheme, document it.

- [ ] **Use version-control software to manage your codebase.**  
  Version-control tooling helps you to collaborate with other contributors and
  ensures provenance tracking of contributions. Moreover it helps you keep
  track of your development and enables you to restore your codebase to a
  former state, in case your codebase gets corrupted. When you publish your
  SOFTWARE, version control is crucial for reproducibility, reusability and
  proper attribution of your team's work.

- [ ] **Keep your codebase simple yet explicit.**  
  Aim for a codebase that is easy to read so as to ease maintenance and lower
  the entry barrier for external contributions. Abide by language-specific
  conventions, recommendations and best practices, and keep the style of your
  codebase consistent. Avoid creating long and/or complicated functions,
  classes and modules, as this will limit their reusability and
  maintainability.

- [ ] **Limit the scope of your SOFTWARE.**  
  Write small tools that perform one task well and refrain from creating a
  "God Software" that tries to do everything all at once. Maintainability is
  one of the core principles of FAIR-RNA, and it quickly becomes impossible
  when your codebase is growing and diversifying too much. For the same
  reason, and to reduce development time, do resist the urge to add
  _potentially useful_ features to your SOFTWARE; wait until they are actually
  requested by USER.

- [ ] **Implement intuitive programmable and extensible APIs for your SOFTWARE.**  
  Ensure modularity of your SOFTWARE by precisely defining in- and outputs, and
  any adjustable parameters. To maximize reusability, do not "hardcode"
  parameters. Abide by API-specific conventions and best practices wherever
  possible. Keeping your APIs simple and intuitive will increase usability and
  thus adoption.

- [ ] **Use standardized input and output formats wherever possible.**  
  Standardized file and other input/output formats are a prerequisite for
  modularity and reusability, and thus sustainable software engineering.
  Consult available ontologies for formats common in your research domain. If
  your data cannot be represented in an available standardized format, try to
  extend an existing format (e.g., by adding additional columns to a
  well-defined table-like file format). If you require extended or custom
  formats for your inputs and outputs, write detailed and unambiguous
  specifications for them and publish them.

- [ ] **Provide informative log, debug and error messages.**  
  Any non-trivial software will contain bugs. Making extensive use of
  informative log messages will save yourself and your USER frustration and
  valuable time in finding out what went wrong if something unforeseen
  happens. Make sure not to leak sensitive information to logs.

- [ ] **Use workflow languages to connect individual processing steps.**  
  If your SOFTWARE project is the development of workflow, it is essential that
  the sequence of individual analysis steps be reproducible. Do not string
  together individual tools with custom wrapper scripts, but instead, use an
  existing well-maintained workflow language/engine that meets FAIR-RNA
  guidelines with respect to reusability, interoperability, maintainability,
  and community involvement/usage.

- [ ] **Document your SOFTWARE and keep documentation up-to-date.**  
  Describe in detail how your SOFTWARE can be used. Aim for a level of
  description that enables USER with basic programming knowledge to run your
  SOFTWARE. Comment critical portions of your code. Keep in mind that USER,
  your successor, or you yourself in the future will have difficulties in
  figuring out the rationale underlying tricky bits of code. Refrain from
  overcommenting your codebase, as it bears the risk of comments and code
  diverging over time. The code remains the ultimate source of truth.

- [ ] **Continuously test your SOFTWARE and ship your tests.**  
  Testing your codebase increases the robustness of your SOFTWARE by ensuring
  stable performance and consistency of outputs. Continuosly running tests for
  any new code to be merged into your codebase may effectively prevent your
  codebase from regressing. Make sure that all elements of your code are
  tested by implementing both unit and integration tests that ideally run every
  line of your code. If you have encountered a bug in your SOFTWARE and
  managed to fix it, add one or more specific tests for that bug to your test
  suite. Make sure to also provide meaningful tests for USER to verify
  installation/deployment success and familiarize themselves with your
  SOFTWARE.

#### Building, packaging & publishing

- [ ] **Provide a simple build mechanism for your SOFTWARE and document it.**  
  To facilitate interoperability, packaging of your SOFTWARE, ideally with all
  dependencies, is required. Apart from language- and domain-specific package
  management systems, which help DEVELOPER in ensuring that their software and
  dependencies will be properly installed and set up, we strongly recommend
  containerizing your SOFTWARE, as this automatically cloud-enables it and
  provides a means for packaging it that is irrespective of programming
  languages and, to some extent, operating systems.

- [ ] **Automate building and publishing and adopt a fast release cycle.**  
  Containerization as described above will also facilitate continuous
  integration and delivery (CI/CD) approaches, which are crucial to the
  robust growth of your SOFTWARE. By committing to a CI/CD solution, changes
  you make to your code can automatically be built, tested and, if all tests
  were successful, delivered (e.g., published or deployed). In this way, new
  features or bug fixes added to your SOFTWARE can be rolled out to USER
  frequently, speeding up the release cycle and your ability to quickly adapt
  and react to current developments and USER requests, respectively.

- [ ] **Obtain a citable identifier for your SOFTWARE.**  
  Distributing your SOFTWARE with a persistent citable identifier establishes
  it as a tool of scholarly interest. This identifier should be easily
  findable, and should interconnect the relevant items, such as your SOFTWARE,
  corresponding publications and authors. Such an identifier also enables
  tracking the usage of your SOFTWARE in the literature, enabling meta-analysis
  and oversight.

- [ ] **Publish your SOFTWARE in one or more suitable repositories.**  
  Using centralized and well established in-domain repositories facilitates
  adoption of your SOFTWARE by the community. You should prefer those
  repositories that adhere with [FAIR Principles][fair] and offer tooling that
  helps both you and USER to comply with FAIR-RNA guidelines.

- [ ] **Provide FAIR metadata relevant for your SOFTWARE.**  
  Consult the [FAIR principles for research software][fair-software] to gain
  insights into which metadata might be relevant to your SOFTWARE. There are
  several ongoing initiatives like [Bioschemas][bioschemas] that are developing
  ontologies for human and machine readable metadata. As a minimum requirement
  we recommend to include source code location, contributors, license,
  references, how to cite the SOFTWARE and a concise description of what the
  SOFTWARE does, as recommended to the [4OSS Recommendations][4oss].

- [ ] **Ensure all contributors are given fair credit for their work.**  
  Adhering to this fundamental principle is the first step towards a fair (and
  [FAIR][fair]) research environment. It will also keep your contributors happy
  and add to your reputation as a reliable collaborator.

- [ ] **Let your SOFTWARE die gracefully.**  
  When you are unable to further maintain SOFTWARE alone or with the help of
  the community, you should communicate this clearly to USER. If your SOFTWARE
  becomes redundant, e.g., because it been entirely superseded by another one,
  you should further deprecate its use entirely. In any case, your SOFTWARE
  should still be available for benchmarking or reproducibility studies.

### For USER

> Follow these guidelines if you are using SOFTWARE as is, without making
> any modifications.

- [ ] **Prefer SOFTWARE that complies with FAIR-RNA guidelines.**  
  By using, citing and recommending compliant SOFTWARE you actively participate
  in creating a FAIRer community as you will incentivize DEVELOPER to adhere
  to these guidelines and thus increase their overall adoption. Be wary of
  using SOFTWARE that is not transparent, unfree or ill-described, as it may
  negatively affect your research and, ultimately, credibility.

- [ ] **Comply with the licensing terms of any SOFTWARE you use.**  
  Respect the intellectual property of DEVELOPER and their freedom to choose
  the terms under which they publish a SOFTWARE, even if you do not personally
  agree with their choice. Do not use a SOFTWARE if you cannot or do not want
  to comply with its licensing terms. Do, however, leave feedback to DEVELOPER
  to encourage them to embrace Free and Open Source SOFTWARE.

- [ ] **Cite all used SOFTWARE.**  
  Software development is hard work and as essential to the advancement of
  science as are new findings or methods. Do respect the time, skills,
  creativity and passion that went into writing every piece of SOFTWARE and
  allow others to fully understand your methodology by giving the deserved
  credit.

- [ ] **Report used versions of all SOFTWARE.**  
  SOFTWARE may develop rapidly, and different versions often will not produce
  the same results or implement the same API that was the foundation of your
  work, so reporting a SOFTWARE without complete version information severly
  limits its reproducibility.

- [ ] **List all non-default parameters that were used and justify their choice.**  
  SOFTWARE frequently allows USER to specify parameters that influence its
  behavior. Thus, without knowing the values of these parameters, it is not
  possible to understand your methodology and reproduce your work. Note also
  that the choice of parameters needs to follow a rationale - do not just try
  different values at random and see what looks best, as this is unscientific.
  Instead, for every non-trivial/-obvious parameter, justify your choice of
  values.

- [ ] **Report details of your runtime environment.**  
  Next to versions and parameters, the identity of other software, such as the
  operating system and any dependencies of your used SOFTWARE, and even
  hardware, may influence the outcome of a SOFTWARE. While it is challenging
  and impractical to capture and report the exact state of your system at the
  time of usage, you should try to get an understanding of the factors that may
  influence the results of running a specific SOFTWARE and then report the
  state of these factors to maximize reproducibility and relevance or general
  applicability of your findings.

### For PUBLISHER

> PUBLISHER includes code hosting services, specialized repositories for
> SOFTWARE, and scientific journals.

- [ ] **Comply with [FAIR Principles][fair].**  
  Ensure that the published SOFTWARE is findable, accessible, interoperable and
  reusable by assigning, among others, the SOFTWARE a globally unique and
  persistent identifier, that the SOFTWARE is indexed in a searchable resource,
  that the SOFTWARE can be accessed through a free and standardized
  communications protocol, and that the SOFTWARE can be (and is encouraged or
  requested to be) described with rich machine-readable metadata by
  contributors.

- [ ] **Encourage that SOFTWARE comply with FAIR-RNA guidelines.**  
  SOFTWARE that adheres to the FAIR-RNA guidelines is likely to be more
  maintainable, sustainable, error-free and of an overall better quality than
  SOFTWARE that follows only a few or none of these guidelines. By encouraging
  adherence to FAIR-RNA guidelines you will therefore host better SOFTWARE and
  thus increase the relevance and quality of your own service.

- [ ] **Provide infrastructure to support FAIR-RNA guidelines.**  
  Make it easy for DEVELOPER to contribute SOFTWARE to your service that
  complies with FAIR-RNA guidelines. Depending on the type of service (hosting
  code vs hosting packaged SOFTWARE vs hosting a publication that describes a
  SOFTWARE), useful tooling to support FAIR-RNA will be different in many
  cases, but should at the very least include an intuitive API (e.g., REST/HTTP
  API) that allows contributors to submit SOFTWARE programmatically.

[4oss]: <https://softdev4research.github.io/recommendations/>
[bioschemas]: <https://bioschemas.org/>
[edam]: <http://edamontology.org>
[fair]: <https://www.go-fair.org/fair-principles/>
[fair-software]: <https://content.iospress.com/articles/data-science/ds190026>
[semver]: <https://semver.org/>
