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
- [System Modelling and Design Using Event-B](https://wiki.event-b.org/images/SM%26D-KAR.pdf) - Ken Robinson's free, book-length introductory notes on modelling with Event-B (PDF).
- [Rodin Handbook](https://stups.hhu-hosting.de/handbook/rodin/current/html/) - Comprehensive guide to installing and using Rodin and Event-B.

## Cheat Sheets and Reference

- [The Event-B Mathematical Language](https://web-archive.southampton.ac.uk/deploy-eprints.ecs.soton.ac.uk/11/4/kernel_lang.pdf) - Metayer and Voisin's formal definition of the Event-B kernel language (PDF).
- [Event-B Mathematical Toolkit Summary](https://wiki.event-b.org/images/EventB-Summary.pdf) - Concise summary of the toolkit with both Rodin and ASCII notation (PDF).
- [Event-B Reference Card](https://wiki.event-b.org/images/EventB-Summary-refcard.pdf) - Quick-reference card for Event-B notation and machine structure (PDF).

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

- [Rodin: an open toolset for modelling and reasoning in Event-B](https://link.springer.com/article/10.1007/s10009-010-0145-y) - Seminal paper describing the Rodin platform.
- [Applying a Formal Method in Industry: a 25-Year Trajectory](https://arxiv.org/abs/2005.07190) - Experience report on B and Event-B in industrial projects.
- [Dependability-Explicit Engineering with Event-B](https://arxiv.org/abs/1210.7032) - Overview of achievements from the EU DEPLOY project.
- [Security Policy Modeling and Verification](https://www.ispras.ru/publications/2018/security_policy_modeling_and_verification/) - ISP RAS work on Event-B modelling and verification of operating-system access-control policies.
- [Jean-Raymond Abrial: A Scientific Biography of a Formal Methods Pioneer](https://arxiv.org/abs/2604.07353) - Biography of the creator of Z, B, and Event-B.

## Standards

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

## Related

- [Awesome TLA+](https://github.com/tlaplus/awesome-tlaplus) - Curated list for the TLA+ formal specification language.
- [Atelier B](https://www.atelierb.eu/en/) - Industrial toolset for the classical B method, Event-B's predecessor.
- [TLA+](https://lamport.azurewebsites.net/tla/tla.html) - Leslie Lamport's language for specifying concurrent and distributed systems.
- [Alloy](https://alloytools.org/) - Lightweight relational modelling language and analyzer.
- [Overture (VDM)](http://overturetool.org/) - Tool support for the Vienna Development Method.
- [Z notation](https://en.wikipedia.org/wiki/Z_notation) - Specification language based on set theory and predicate logic.

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) first.
