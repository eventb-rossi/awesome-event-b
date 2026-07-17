# Awesome Event-B [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of resources for the Event-B formal method and the Rodin platform.

Event-B is a formal method for system-level modelling and analysis. It uses set theory as a notation, refinement to relate models at different levels of abstraction, and mathematical proof to verify their consistency. Models are built and proofs discharged in the open, Eclipse-based Rodin platform. The method was created by Jean-Raymond Abrial and is widely applied to safety-critical systems such as railway signalling.

## Contents

- [Official Resources](#official-resources)
- [Tools](#tools)
  - [Platform](#platform)
  - [Command-Line and Tooling](#command-line-and-tooling)
  - [Editors](#editors)
  - [Provers and Verification](#provers-and-verification)
  - [Animation and Visualization](#animation-and-visualization)
  - [Modelling Extensions](#modelling-extensions)
  - [Code Generation](#code-generation)
  - [Requirements and Documentation](#requirements-and-documentation)
- [Books](#books)
- [Cheat Sheets and Reference](#cheat-sheets-and-reference)
- [Tutorials](#tutorials)
- [Models and Examples](#models-and-examples)
- [Papers](#papers)
  - [Foundations and Methodology](#foundations-and-methodology)
  - [Tools and Verification](#tools-and-verification)
  - [Applications and Case Studies](#applications-and-case-studies)
- [Standards](#standards)
- [Conferences](#conferences)
- [Community](#community)
- [Industrial Use](#industrial-use)
- [Related](#related)

## Official Resources

- [Event-B and Rodin Wiki](https://wiki.event-b.org/index.php/Main_Page) - Community-maintained hub for the language, platform, tutorials, and plugins.
- [Event-B Language](https://wiki.event-b.org/index.php/Event-B_Language) - Reference for the Event-B mathematical notation and model structure.
- [Rodin Platform Welcome Page](https://wiki.event-b.org/index.php/Rodin_Platform_Welcome_Page) - Starting point with downloads and getting-started material.
- [Rodin Platform Releases](https://wiki.event-b.org/index.php/Rodin_Platform_Releases) - Version history and release notes for the Rodin toolset.
- [Event-B on Wikipedia](https://en.wikipedia.org/wiki/Event-B) - Concise encyclopedic introduction to the method and its background.

## Tools

### Platform

- [Rodin](https://sourceforge.net/projects/rodin-b-sharp/) - Eclipse-based IDE for modelling, refinement, and proof in Event-B.
- [RodinCore](https://github.com/systerel/RodinCore) - Source repository for the Rodin platform core.
- [Rodin Plug-ins](https://wiki.event-b.org/index.php/Rodin_Plug-ins) - Index of available plugins with descriptions and install sites.

### Command-Line and Tooling

- [Rossi](https://eventb-rossi.org/) - Rust toolchain for Event-B with a parser, type checker, CLI, and language server that round-trips with Rodin.
- [rodin-headless](https://github.com/eventb-rossi/rodin-headless) - Headless toolchain to build, model-check, and prove Rodin Event-B models from the command line or Docker.
- [eventb-animate](https://github.com/eventb-rossi/eventb-animate) - Command-line tool to animate Event-B models with ProB without Rodin.
- [eventb-checker](https://github.com/eventb-rossi/eventb-checker) - Command-line validator for Event-B models, also available as a GitHub Action.
- [eventb-to-txt](https://github.com/eventb-rossi/eventb-to-txt) - Converts Event-B machines and contexts to CamilleX plain-text models.
- [tree-sitter-eventb](https://github.com/eventb-rossi/tree-sitter-eventb) - Tree-sitter grammar for the Event-B textual syntax, generated from Rossi.

### Editors

- [Event-B for VS Code](https://marketplace.visualstudio.com/items?itemName=rossi.event-b) - VS Code extension for Event-B with syntax highlighting and the Rossi language server, also on [Open VSX](https://open-vsx.org/extension/rossi/event-b).

### Provers and Verification

- [SMT Solvers Plug-in](https://wiki.event-b.org/index.php/SMT_Solvers_Plug-in) - Discharges proof obligations using external SMT solvers.
- [Isabelle for Rodin](https://wiki.event-b.org/index.php/Isabelle_for_Rodin) - Integrates the Isabelle/HOL prover with Event-B proofs.

### Animation and Visualization

- [ProB](https://prob.hhu.de/) - Animator and model checker for Event-B, B, Z, TLA+, and CSP.
- [ProB2-UI](https://github.com/hhu-stups/prob2_ui) - Modern JavaFX interface for the ProB animator and model checker.
- [VisB](https://prob.hhu.de/w/index.php?title=VisB) - Adds lightweight SVG-based visualizations to formal models.
- [SimB](https://prob.hhu.de/w/index.php?title=SimB) - Timed, probabilistic simulation of Event-B models.
- [AnimB](https://wiki.event-b.org/index.php/AnimB) - Animator for stepping through Event-B models inside Rodin.
- [BMotionWeb](https://prob.hhu.de/w/index.php?title=BMotionWeb) - Builds domain-specific, web-based visualizations of formal models.

### Modelling Extensions

- [Theory Plug-in](https://wiki.event-b.org/index.php/Theory_Plug-in) - Extends the mathematical language with operators, datatypes, and rewrite rules.
- [UML-B](https://www.uml-b.org/) - Diagrammatic class- and state-machine front end for Event-B.
- [CamilleX](https://wiki.event-b.org/index.php/CamilleX) - Text-based editor and syntax extensions for Event-B.
- [Records Extension](https://wiki.event-b.org/index.php/Records_Extension) - Adds structured record types to the Event-B language.
- [Decomposition Plug-in](https://wiki.event-b.org/index.php/Decomposition_Plug-in_User_Guide) - Splits a model into sub-models via shared variables or events.
- [Atomicity Decomposition Plug-in](https://wiki.event-b.org/index.php/Atomicity_Decomposition_Plug-in_User_Guide) - Structures the refinement of event atomicity.
- [Modularisation Plug-in](https://wiki.event-b.org/index.php/Modularisation_Plug-in) - Builds and proves modular Event-B developments.
- [Flows Plug-in](https://wiki.event-b.org/index.php/Flows) - Adds explicit control flow between events.

### Code Generation

- [Code Generation Activity](https://wiki.event-b.org/index.php/Code_Generation_Activity) - Overview of code generation approaches and tools for Event-B.
- [Tasking Event-B](https://wiki.event-b.org/index.php/Tasking_Event-B_Overview) - Generates multi-tasking code in Ada, Java, and C from Event-B.

### Requirements and Documentation

- [ProR](https://wiki.event-b.org/index.php/ProR) - Links natural-language requirements to Event-B models.
- [B2Latex](https://wiki.event-b.org/index.php/B2Latex) - Typesets Event-B models as LaTeX for documents.

## Books

- [Modeling in Event-B: System and Software Engineering](https://www.cambridge.org/core/books/modeling-in-eventb/F39FF5F1B60F0AA585718B8E6A4F9DD7) - Jean-Raymond Abrial's definitive textbook on the method.
- [System Modelling and Design Using Event-B](https://wiki.event-b.org/images/SM%26D-KAR.pdf) - Ken Robinson's free, book-length introductory notes on modelling with Event-B (PDF, [archived](https://web.archive.org/web/20260606061302/https://wiki.event-b.org/images/SM%26D-KAR.pdf)).
- [Rodin Handbook](https://stups.hhu-hosting.de/handbook/rodin/current/html/) - Comprehensive guide to installing and using Rodin and Event-B.
- [A Tool's Security Model: Formally Describing Software Subsystems](https://books.ifmo.ru/file/pdf/3025.pdf) - Begaev and colleagues' Russian-language ITMO University study guide on building a software security model in Event-B with iUML-B and Rodin for FSTEC certification (PDF, [archived](https://web.archive.org/web/20220429054626/https://books.ifmo.ru/file/pdf/3025.pdf)).

## Cheat Sheets and Reference

- [The Event-B Mathematical Language](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/11/4/kernel_lang.pdf) - Metayer and Voisin's formal definition of the Event-B kernel language (PDF, [archived](https://web.archive.org/web/20220119135226/http://deploy-eprints.ecs.soton.ac.uk/11/4/kernel_lang.pdf)).
- [Event-B Mathematical Toolkit Summary](https://wiki.event-b.org/images/EventB-Summary.pdf) - Concise summary of the toolkit with both Rodin and ASCII notation (PDF, [archived](https://web.archive.org/web/20260508084901/https://wiki.event-b.org/images/EventB-Summary.pdf)).
- [Event-B Reference Card](https://wiki.event-b.org/images/EventB-Summary-refcard.pdf) - Quick-reference card for Event-B notation and machine structure (PDF, [archived](https://web.archive.org/web/20260508090649/https://wiki.event-b.org/images/EventB-Summary-refcard.pdf)).

## Tutorials

- [Rodin Tutorials](https://wiki.event-b.org/index.php/Rodin_Tutorials) - Index of official tutorials for Rodin and its plugins.
- [ProB First Steps](https://prob.hhu.de/w/index.php?title=Tutorial_Rodin_First_Step) - Hands-on introduction to animating Event-B with ProB.
- [UML-B Tutorial](https://wiki.event-b.org/index.php/UML-B_Tutorial) - Step-by-step guide to diagrammatic modelling with UML-B.

## Models and Examples

- [Event-B Examples](https://wiki.event-b.org/index.php/Event-B_Examples) - Community index of downloadable Event-B developments, from teaching to industrial.
- [Industrial Projects](https://wiki.event-b.org/index.php/Industrial_Projects) - Wiki overview of industrial projects and companies that have applied Event-B.
- [DEPLOY Examples Archive](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/view/subjects/examples.html) - Archived repository of 60+ Event-B case studies from the EU DEPLOY project.
- [ARINC 653](https://github.com/LVPGroup/arinc653model) - Event-B formalization of the ARINC 653 avionics OS standard that uncovered six specification issues (ISSRE 2015).
- [Landing Gear System](https://abz-conf.org/case-study/abz14/) - Aircraft landing gear, the benchmark case study of ABZ 2014, with several Event-B solutions.
- [Hybrid ERTMS/ETCS Level 3](https://abz-conf.org/case-study/abz18/) - European railway moving-block signalling, the benchmark case study of ABZ 2018.
- [Adaptive Exterior Light and Speed Control](https://github.com/hhu-stups/abz2020-models) - Automotive light and speed controller with a pitman-arm lever, the ABZ 2020 case study with Rodin models.
- [HIMACF Access Control Model](https://github.com/eventb-rossi/rbac-model) - Event-B specification of the role-based access control and information-flow model (formerly MROSL DP-model) used in Astra Linux.
- [Mondex Electronic Purse](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/38/index.html) - Incremental Event-B refinement of the Mondex smartcard electronic purse, a classic verification benchmark.
- [CDIS Air-Traffic Information System](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/9/index.html) - Event-B redevelopment of a commercial air-traffic control information system first specified in VDM.
- [Reconfigurable On-Board Satellite System](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/411/index.html) - Formal development and dependability assessment of a reconfigurable satellite system from the DEPLOY space pilot.
- [Cruise Control System](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/209/index.html) - Event-B modelling of an automotive cruise-control system used to evaluate a modelling guideline.
- [Mechanical Press Controller](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/113/index.html) - Refinement-based Event-B development of an industrial mechanical-press controller.

## Papers

### Foundations and Methodology

- [Refinement, Decomposition, and Instantiation of Discrete Models](https://content.iospress.com/articles/fundamenta-informaticae/fi77-1-2-02) - Abrial and Hallerstede's foundational account of refinement, decomposition, and generic instantiation in Event-B.
- [An Open Extensible Tool Environment for Event-B](https://link.springer.com/chapter/10.1007/11901433_32) - Early paper introducing the extensible Event-B tool environment that grew into the Rodin platform.
- [On the Purpose of Event-B Proof Obligations](https://link.springer.com/article/10.1007/s00165-009-0138-3) - Hallerstede's explanation of how Event-B's proof obligations encode the method's semantics.
- [The Logic of Event-B](https://www.research-collection.ethz.ch/handle/20.500.11850/69354) - Schmalz's specification of Event-B's abstract syntax, three-valued semantics, and proof calculus (ETH Technical Report 698).
- [Term Rewriting in Logics of Partial Functions](https://www.research-collection.ethz.ch/handle/20.500.11850/69779) - Schmalz's report on rewriting and well-definedness in the partial-function logic underlying Event-B proofs.
- [Reasoning about Liveness Properties in Event-B](https://link.springer.com/chapter/10.1007/978-3-642-24559-6_31) - Hoang and Abrial's proof rules for liveness properties under Event-B refinement.
- [Decomposition Structures for Event-B](https://link.springer.com/chapter/10.1007/978-3-642-00255-7_2) - Butler's atomicity decomposition and event-refinement diagrams for structuring large refinements.
- [Practical Theory Extension in Event-B](https://link.springer.com/chapter/10.1007/978-3-642-39698-4_5) - Butler and Maamria on the Theory plug-in for extending Event-B's mathematical language.
- [Faultless Systems: Yes We Can!](https://ieeexplore.ieee.org/document/5233504) - Abrial's manifesto arguing that proof-based development can deliver fault-free systems.
- [Jean-Raymond Abrial: A Scientific Biography of a Formal Methods Pioneer](https://arxiv.org/abs/2604.07353) - Biography of the creator of Z, B, and Event-B.

### Tools and Verification

- [Rodin: an open toolset for modelling and reasoning in Event-B](https://link.springer.com/article/10.1007/s10009-010-0145-y) - Seminal paper describing the Rodin platform.
- [ProB: A Model Checker for B](https://link.springer.com/chapter/10.1007/978-3-540-45236-2_46) - Leuschel and Butler's widely cited model checker and animator for B and Event-B.
- [ProB: An Automated Analysis Toolset for the B Method](https://link.springer.com/article/10.1007/s10009-007-0063-9) - Journal account of the ProB toolset for animation, model checking, and refinement checking.
- [Integrating SMT Solvers in Rodin](https://doi.org/10.1016/j.scico.2014.04.012) - Deharbe and colleagues on discharging Event-B proof obligations with SMT solvers.
- [Automatic Code Generation from Event-B Models](https://inria.hal.science/inria-00637765) - Mery and Singh's EB2ALL approach to generating C, C++, Java, and C# from Event-B models.

### Applications and Case Studies

- [Applying a Formal Method in Industry: a 25-Year Trajectory](https://arxiv.org/abs/2005.07190) - Experience report on B and Event-B in industrial projects.
- [Dependability-Explicit Engineering with Event-B](https://arxiv.org/abs/1210.7032) - Overview of achievements from the EU DEPLOY project.
- [An Incremental Development of the Mondex System in Event-B](https://link.springer.com/article/10.1007/s00165-007-0061-4) - Butler and Yadav's refinement-based development of the Mondex electronic purse, a verification benchmark.
- [A Mechanically Proved and Incremental Development of IEEE 1394 Tree Identify Protocol](https://inria.hal.science/inria-00099531) - Abrial, Cansell, and Mery's proved development of the FireWire tree-identify protocol.
- [Pacemaker's Functional Behaviors in Event-B](https://inria.hal.science/inria-00419973) - Mery and Singh's incremental Event-B model of a cardiac pacemaker's functional behaviour.
- [Event-Based Formalization of ARINC 653 using Event-B](https://arxiv.org/abs/1508.06479) - Zhao and colleagues' formalisation of the ARINC 653 avionics OS standard (ISSRE 2015).
- [Security Policy Modeling and Verification](https://www.ispras.ru/publications/2018/security_policy_modeling_and_verification/) - ISP RAS work on Event-B modelling of operating-system access-control policies.

## Standards

- [CENELEC EN 50128:2011+A2:2020](https://landingpage.bsigroup.com/LandingPage/Standard?UPI=000000000030415465) - European railway-software standard whose informative Annex D.28.9 describes Event B as the system-modelling branch of the B method. The [current successor, EN 50716:2023](https://www.nek.no/wp-content/uploads/2025/03/nek-en-50716_2023_en_001.pdf), retains the B method.
- [IEC 62279:2015](https://webstore.iec.ch/en/publication/22781) - International counterpart to EN 50128; informative Annex D.28.9 contains the same explicit description of Event B.
- [GOST R IEC 62279-2016](https://protect.gost.ru/gost/details/639bf6b0-c641-4845-a717-97638cb7e40b) - Active, identical Russian adoption of IEC 62279:2015 for railway software. Its [Annex D.28.10](https://meganorm.ru/mega_doc/norm/gost-r_gosudarstvennyj-standart/14/gost_r_mek_62279-2016_natsionalnyy_standart_rossiyskoy.html) explicitly describes Event-B as “Событие B”.
- [GB/T 28808-2021](https://std.samr.gov.cn/gb/search/gbDetailed?id=D4BEFFF4EA39B241E05397BE0A0AF581) - Current Chinese railway-software standard and modified adoption of IEC 62279:2015. Its informative Annex B corresponds to IEC Annex D, including the Event B description.
- [NITE Railway Accreditation Scope](https://www.nite.go.jp/data/000072146.pdf) - Japanese accreditation scope that includes IEC 62279:2015; an [IPA case-study report](https://www.ipa.go.jp/archive/files/000004620.pdf) separately documents Event-B and Rodin use in Japan.
- [GOST R 59453.1-2021](https://protect.gost.ru/gost/details/3fa98ad7-e0ac-4f80-8fe2-5eebace2b3f7) - Russian national standard on the formal access-control model, general provisions.
- [GOST R 59453.2-2021](https://base.garant.ru/401555448/) - Companion standard that recommends Event-B among formalization methods and Rodin as an example tool, with worked Event-B verification examples.

## Conferences

- [ABZ](https://abz-conf.org/) - Conference for state-based methods including ASM, Alloy, B, TLA, VDM, Z, and Event-B.
- [Formal Methods Europe](https://www.fmeurope.org/) - Organisation behind the FM and integrated formal-methods conferences.

## Community

- [Mailing Lists](https://wiki.event-b.org/index.php/Mailing_lists) - Announce, user, and developer lists for Rodin and Event-B.
- [Rodin User List Archive](https://sourceforge.net/p/rodin-b-sharp/mailman/rodin-b-sharp-user/) - Searchable archive of the Rodin user mailing list.
- [HHU STUPS](https://github.com/hhu-stups) - Research group developing ProB and related Event-B tooling.

## Industrial Use

- [Systerel](https://www.systerel.fr/en/) - Company leading Rodin platform development and formal verification services.
- [ClearSy](https://www.clearsy.com/en/) - Engineering firm applying B and Event-B to railway safety systems.
- [openETCS Model Evaluation](https://github.com/openETCS/model-evaluation) - Event-B models from the openETCS railway standardisation initiative.
- [AstraVer Toolset](https://www.ispras.ru/en/projects/astraver_toolset/) - ISP RAS toolset that verifies Astra Linux security modules, pairing C deductive verification with Event-B security-policy models in Rodin.

## Related

- [Awesome TLA+](https://github.com/tlaplus/awesome-tlaplus) - Curated list for the TLA+ formal specification language.
- [Atelier B](https://www.atelierb.eu/en/) - Industrial toolset for the classical B method, Event-B's predecessor.
- [TLA+](https://lamport.azurewebsites.net/tla/tla.html) - Leslie Lamport's language for specifying concurrent and distributed systems.
- [Alloy](https://alloytools.org/) - Lightweight relational modelling language and analyzer.
- [Overture (VDM)](http://overturetool.org/) - Tool support for the Vienna Development Method.
- [Z notation](https://en.wikipedia.org/wiki/Z_notation) - Specification language based on set theory and predicate logic.

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) first.
