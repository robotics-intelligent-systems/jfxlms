# jfxlms --- OpenTwin AI Learning Management & Digital Education Platform

> Open, modular reference architecture for AI-assisted learning, LMS
> interoperability, adaptive education, real-time collaboration, STEM
> learning, open educational resources, analytics, simulation, and
> educational digital twins.

## Description and Context

**jfxlms / OpenTwin AI Learning Management & Digital Education
Platform** consolidates the jfxlms technology compendium into a
structured open architecture for learning management, AI-assisted
education, adaptive tutoring, assessment, collaboration, interactive
STEM, content authoring, analytics and educational digital twins.

The source project references BigBlueButton, OpenTutor, PenEcho,
SwallowCode, SwallowMath, Interactive OpenMP Programming, ocp-reveal,
Frappe Learning, OCW Management System, Presenton, Llemma, GeoGebra,
React SCORM Provider, OpenOlat, eXeLearning, Adapt Framework, Forma LMS,
CourseLit, OpenBoard, MathQuill, MathJax, Artemis, Liferay Portal,
Sakai, Moodle-to-edX conversion, Canvas, Odoo eLearning and OpenVidu.

This consolidation classifies technologies as **required dependencies,
optional integrations, or research references**, rather than assuming
one mandatory runtime stack.

**Design principle:** open, modular architecture designed to minimize
proprietary lock-in and enable independent implementations.

## Vision

``` text
LEARNERS / TEACHERS / TUTORS / INSTITUTIONS
                    |
           LEARNING EXPERIENCE
                    |
       Courses / Classes / Assessments
                    |
          AI TUTOR & AGENTS
                    |
 RAG / Adaptation / Feedback / Analytics
                    |
          OPENTWIN LEARNING CORE
                    |
 Learner Twin / Course Twin / Skill Twin / Lab Twin
                    |
 LMS / SCORM / LTI / xAPI / WebRTC / Content
                    |
 Knowledge / Events / Assessments / Records
                    |
          MBSE / SIMULATION / LABS
```

## Objectives

-   Provide a modular learning-management reference architecture.
-   Support self-paced, instructor-led and blended learning.
-   Integrate AI tutoring with pedagogical and human oversight.
-   Enable adaptive learning and personalized study paths.
-   Represent courses, skills, laboratories and learning state through
    digital twins.
-   Support mathematics, programming and engineering education.
-   Integrate synchronous classes, shared whiteboards and collaboration.
-   Support reusable open educational resources.
-   Provide standards-oriented LMS interoperability.
-   Enable privacy-aware learning analytics.
-   Keep LMS, conferencing, AI and content components replaceable.
-   Preserve MBSE and simulation in the engineering lifecycle.
-   Avoid mandatory dependence on a proprietary LMS, cloud or AI
    provider.

## Reference Architecture

``` text
EXPERIENCE
Learner | Teacher | Tutor | Author | Administrator
                         |
LEARNING SERVICES
Courses | Classes | Assessments | Content | Labs
Collaboration | Credentials | Feedback | Tutoring
                         |
OPENTWIN LEARNING CORE
Twin Registry | State | Skills | Events | Provenance
                         |
AI & ADAPTIVE LEARNING
Tutor | RAG | Recommendations | Feedback | Analytics
                         |
INTEROPERABILITY
LMS APIs | SCORM | LTI | xAPI | WebRTC | Content
                         |
DATA & KNOWLEDGE
SQL | Objects | Events | Learning Records | Vector Data
```

Cross-cutting concerns: **Identity · Accessibility · Privacy · Security
· Responsible AI · Provenance · Observability · Portability · Open
Licensing**.

## OpenTwin Learning Model

Candidate twins include:

-   Learner Twin
-   Course Twin
-   Skill/Competency Twin
-   Learning Path Twin
-   Assessment Twin
-   Laboratory Twin
-   Classroom Twin
-   Learning Resource Twin
-   Cohort Twin
-   Educational Infrastructure Twin

``` text
Learning Activity
       |
LMS / Lab / Assessment / Collaboration
       |
Event Adapter
       |
OpenTwin Learning Core
       |
Current State + History + Evidence
       |
Skills / Goals / Analytics
       |
Recommendation / Feedback
       |
Teacher / Learner Review
```

Example:

``` yaml
twin:
  id: learner-example-001
  type: learner
  state:
    enrolled_courses: []
    competencies: []
    learning_goals: []
    progress: {}
  evidence_refs: []
  activity_refs: []
  recommendations: []
  provenance: {}
```

A Learner Twin is a computational educational representation, not a
complete representation of a person. Sensitive learner information
should be minimized and governed separately from ordinary platform
telemetry.

## Learning Management Core

Candidate capabilities include course catalogs, enrollment, cohorts,
lessons/modules, prerequisites, assignments, quizzes, gradebooks,
completion tracking, certificates, notifications, calendars,
discussions, dashboards and administrative reporting.

``` text
Catalog -> Enrollment -> Learning Path
        -> Content / Class / Lab
        -> Assessment -> Feedback
        -> Progress / Credential
```

## AI Tutoring and Adaptive Learning

Potential functions:

-   conversational tutoring;
-   question answering over approved course materials;
-   adaptive exercise selection;
-   formative feedback and hints;
-   rubric-assisted feedback;
-   content summarization;
-   multilingual learning support;
-   programming and mathematics assistance;
-   study-plan generation;
-   knowledge-gap identification.

``` text
Approved Learning Content
          |
       Retrieval
          |
    AI Tutor / Rules
          |
 Evidence + Explanation
          |
 Learner Interaction
          |
 Teacher / Policy Oversight
```

AI interactions should retain model/version information, source
provenance, limitations and review status. High-impact educational
decisions should not depend solely on opaque automated scoring.

## Assessment and Feedback

``` text
Learning Objective
       |
Assessment
       |
Learner Submission
       |
Automated + Human Evaluation
       |
Feedback / Evidence
       |
Competency Update
```

Assessment may include quizzes, programming exercises, mathematics,
modeling, written assignments, projects, peer assessment and practical
laboratory activities.

## STEM and Interactive Learning

The architecture can support interactive geometry, algebra, calculus,
statistics, mathematical notation, programming exercises,
parallel-computing education, engineering models, simulation
laboratories and shared mathematical whiteboards.

Math rendering/editing and STEM tools should remain replaceable
integrations rather than hard-wired core dependencies.

## Content Authoring and OER

``` text
Author
  |
Course / Lesson Editor
  |
Media + Math + Interactive Components
  |
Packaging / Metadata
  |
Repository
  |
LMS / Web / Offline Distribution
```

Potential capabilities include responsive authoring, presentations,
interactive content, templates, accessible media, mathematical content,
versioning, attribution and open-license metadata.

## Real-Time Collaboration

Potential capabilities include video conferencing, audio, screen
sharing, chat, breakout rooms, shared canvas, interactive whiteboards,
handwriting, equations, diagrams, presence and authorized session
recording.

WebRTC services should be isolated behind collaboration interfaces.

## Interoperability

Potential integration boundaries:

-   LMS REST APIs;
-   SCORM;
-   LTI;
-   xAPI;
-   learning-record stores;
-   WebRTC;
-   content repositories;
-   identity federation;
-   assessment/grade exchange.

``` text
External LMS / Tool
        |
Adapter / Contract
        |
OpenTwin Learning Services
        |
Events / Learning Records
        |
Twin State / Analytics
```

Compatibility should be validated against specific versions and profiles
rather than assumed from protocol names.

## Learning Analytics

Potential analytics include engagement, progress, completion, assessment
performance, competency development, course effectiveness, resource
usage, cohort trends, bottlenecks and tutoring effectiveness.

Analytics should avoid unnecessary surveillance. Data collection should
be proportionate to a defined educational purpose.

## Security, Privacy and Responsible AI

Recommended controls include OIDC/OAuth2-compatible identity, MFA for
privileged roles, RBAC/ABAC, least privilege, encrypted communications,
secrets management, tenant isolation, audit trails, data minimization,
retention controls, appropriate export/deletion workflows, secure
updates, dependency scanning, backup/recovery, AI provenance and human
review for consequential decisions.

Deployments involving minors require particular attention to
age-appropriate privacy, security, safeguarding and applicable
education/data-protection requirements.

## MBSE and Simulation

The source repository organizes engineering around:

``` text
MBSE -> CAD -> CAM -> CAS
```

Arcadia/Capella can structure stakeholder needs, operational analysis,
system analysis, logical architecture, physical architecture,
implementation and verification.

Potential simulation subjects include learner flow, course capacity,
tutoring workloads, virtual-classroom scaling, assessment pipelines,
content delivery, educational infrastructure and adaptive-learning
policies.

## Open-Source Technology Compendium

  ------------------------------------------------------------------------------
  Domain                  Candidate / Reference   Potential Role
  ----------------------- ----------------------- ------------------------------
  Virtual Classroom       BigBlueButton           Web conferencing / online
                                                  classes

  Adaptive Learning       OpenTutor               Adaptive-learning
                                                  research/reference

  Collaborative Canvas    PenEcho                 Handwriting/equation/diagram
                                                  workspace

  AI Dataset              SwallowCode             Programming dataset reference

  AI Dataset              SwallowMath             Mathematics dataset reference

  Programming Education   Interactive OpenMP      LLM/HPC education reference
                          Programming             

  Presentations           ocp-reveal              Presentation technology

  LMS                     Frappe Learning         LMS implementation

  OER / OCW               OCW Management System   Open courseware management

  AI Presentations        Presenton               AI presentation generation

  Mathematical AI         Llemma                  Mathematics model reference

  STEM                    GeoGebra                Interactive mathematics

  SCORM                   React SCORM Provider    SCORM integration

  LMS                     OpenOlat                E-learning platform

  OER Authoring           eXeLearning             OER authoring

  Course Authoring        Adapt Framework         Responsive HTML5 courses

  LMS                     Forma LMS               E-learning platform

  LMS                     CourseLit               Learning-management platform

  Whiteboard              OpenBoard               Interactive whiteboard

  Mathematics             MathQuill               Formula editor

  Mathematics             MathJax                 Math rendering

  Assessment              Artemis                 Exercises and feedback

  Portal                  Liferay Portal          Enterprise portal

  LMS / Collaboration     Sakai                   Teaching/research
                                                  collaboration

  Migration               Moodle-to-edX tooling   Course conversion reference

  LMS                     Canvas                  LMS integration/reference

  LMS / ERP               Odoo eLearning          Learning integration

  Real-Time Media         OpenVidu                WebRTC platform

  MBSE                    Arcadia / Capella       Systems engineering
  ------------------------------------------------------------------------------

Inclusion does not imply endorsement, bundling, mandatory dependency,
current maintenance status, or license/runtime compatibility. Review
each candidate before adoption.

## User Guide

1.  Register an institution/workspace.
2.  Configure identity and roles.
3.  Create courses and learning objectives.
4.  Add resources and activities.
5.  Configure assessments and rubrics.
6.  Enable optional collaboration.
7.  Register learner/course/skill twins.
8.  Connect approved AI tutoring services.
9.  Enroll learners.
10. Collect authorized learning events.
11. Review progress and evidence.
12. Apply teacher/tutor intervention where appropriate.
13. Export records through supported adapters.

## Installation Guide

``` bash
git clone https://github.com/robotics-intelligent-systems/jfxlms.git
cd jfxlms
```

The repository should be treated as a technology compendium/reference
architecture unless an executable module explicitly documents otherwise.
Do not assume every referenced project must be installed.

Minimal target:

``` text
Web Client
    |
Learning Core API
    |
Course / Enrollment / Assessment
    |
PostgreSQL
    |
OpenTwin Learning Registry
```

Extended deployments can add object storage, an event broker,
learning-record store, LMS/SCORM/LTI/xAPI adapters, WebRTC
collaboration, AI tutor/RAG, vector search, analytics, STEM tools and
audit/provenance.

Each executable module should document tested runtime versions, package
managers, environment variables, migrations, networking, storage,
secrets, build steps and tests.

## Dependencies

### Required Dependencies

Only components necessary for the selected executable implementation.

### Optional Integrations

Examples include BigBlueButton, OpenVidu, Frappe Learning, OpenOlat,
Forma LMS, CourseLit, Sakai, Canvas adapters, Odoo eLearning, GeoGebra,
MathJax, MathQuill, Artemis, eXeLearning, Adapt Framework, AI/RAG
components, PostgreSQL, object storage and event brokers.

### Research References

Datasets, models and projects used for architectural comparison or
experimentation without becoming runtime dependencies.

Recommended record:

``` yaml
dependency:
  name:
  version:
  role:
  status: required | optional | reference
  license:
  source:
  tested_platforms:
  security_notes:
  interoperability_notes:
  privacy_notes:
```

## Recommended Repository Structure

``` text
jfxlms/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── CODE_OF_CONDUCT.md
├── docs/
│   ├── architecture/
│   ├── pedagogy/
│   ├── interoperability/
│   ├── security/
│   └── privacy/
├── MBSE/
│   ├── operational/
│   ├── system/
│   ├── logical/
│   ├── physical/
│   └── CAS/
├── core/
│   ├── institutions/
│   ├── courses/
│   ├── enrollment/
│   └── assessments/
├── twins/
│   ├── registry/
│   ├── learner/
│   ├── course/
│   ├── skill/
│   └── lab/
├── ai/
│   ├── tutor/
│   ├── rag/
│   ├── evaluation/
│   └── governance/
├── content/
├── oer/
├── collaboration/
├── stem/
├── analytics/
├── interoperability/
│   ├── scorm/
│   ├── lti/
│   ├── xapi/
│   └── lms/
├── api/
├── events/
├── audit/
├── integrations/
├── simulation/
├── deployment/
├── tests/
└── examples/
```

## MVP

``` text
Learner / Teacher Web UI
           |
    Learning Core API
           |
Courses / Assessments / Twins
           |
       PostgreSQL
```

MVP features:

-   institution/workspace registry;
-   user roles;
-   course catalog;
-   enrollment;
-   lessons/modules;
-   basic assessments;
-   progress tracking;
-   learner/course/skill twin registry;
-   learning events;
-   audit/provenance;
-   REST API;
-   learner/teacher dashboards;
-   containerized local deployment.

Optional MVP+ features include an AI tutor over approved course content,
mathematics integration, virtual-classroom adapter, xAPI/LTI adapter and
simple analytics.

Success criteria: teachers can publish courses; learners can enroll and
complete activities; assessment evidence and progress are auditable;
authorized events can reconstruct twin state; access controls separate
roles; deployment is reproducible; and no proprietary cloud is
mandatory.

## Development Roadmap

### Phase 1 --- Architecture and Documentation

-   [x] BID-inspired documentation structure.
-   [x] Technology-compendium consolidation.
-   [x] OpenTwin learning architecture.
-   [x] Initial dependency classification.
-   [ ] Architecture Decision Records.
-   [ ] Formal domain schemas.

### Phase 2 --- LMS Core

-   [ ] Identity and roles.
-   [ ] Institutions/workspaces.
-   [ ] Courses/modules.
-   [ ] Enrollment.
-   [ ] Assessments/progress.
-   [ ] Audit.

### Phase 3 --- OpenTwin Learning

-   [ ] Twin registry.
-   [ ] Learner/Course/Skill Twins.
-   [ ] Learning-event model.
-   [ ] Provenance.

### Phase 4 --- Interoperability

-   [ ] SCORM.
-   [ ] LTI.
-   [ ] xAPI/LRS.
-   [ ] External LMS adapters.
-   [ ] Content import/export.

### Phase 5 --- Collaboration

-   [ ] Virtual classroom.
-   [ ] WebRTC adapter.
-   [ ] Shared whiteboard.
-   [ ] Collaborative mathematics.

### Phase 6 --- STEM and Virtual Labs

-   [ ] Math rendering/editing.
-   [ ] Interactive mathematics.
-   [ ] Programming exercises.
-   [ ] Engineering simulation.
-   [ ] Virtual laboratories.

### Phase 7 --- AI Tutor

-   [ ] RAG over approved materials.
-   [ ] Tutor orchestration.
-   [ ] Adaptive recommendations.
-   [ ] Model provenance.
-   [ ] Evaluation framework.
-   [ ] Human oversight.

### Phase 8 --- Analytics

-   [ ] Learning/cohort/competency analytics.
-   [ ] Intervention workflows.
-   [ ] Privacy-preserving reporting.

### Phase 9 --- Production Hardening

-   [ ] Observability/high availability.
-   [ ] Backup/recovery.
-   [ ] Security testing.
-   [ ] Accessibility testing.
-   [ ] Privacy assessment.
-   [ ] Load/performance testing.

## How to Contribute

Contributions are welcome in LMS architecture, digital education,
adaptive learning, AI tutoring, RAG, SCORM/LTI/xAPI, STEM education,
virtual labs, assessment, analytics, accessibility, privacy,
cybersecurity, MBSE and documentation.

``` bash
git checkout -b feature/my-contribution
git add .
git commit -m "Add: description of contribution"
git push origin feature/my-contribution
```

Pull requests should describe the problem, solution,
pedagogical/architectural impact, interfaces, dependencies/licenses,
privacy/security implications, accessibility, AI/model implications,
tests and documentation.

Do not commit credentials, private student information, unauthorized
educational records, copyrighted course material without permission, or
restricted datasets.

## Code of Conduct

Maintain a respectful, inclusive, professional and technically
constructive environment. A dedicated `CODE_OF_CONDUCT.md` should be
maintained at repository root.

## Authors and Maintainers

Maintained by the **Robotics Intelligent Systems** open-source
initiative.

Repository: `robotics-intelligent-systems/jfxlms`

Third-party projects, standards, datasets, models, trademarks and
documentation remain the property of their respective owners.

## Additional Information

The project is intended as an open educational-technology compendium,
modular LMS architecture reference, educational digital-twin research
platform, AI-assisted learning foundation and MBSE reference for digital
education systems.

## Intellectual Property and Open Design

OpenTwin Learning favors open standards, documented interfaces, modular
adapters, replaceable implementations, open educational resources where
licensing permits, explicit provenance and reproducible engineering
artifacts.

The goal is to minimize proprietary lock-in and enable independently
developed compatible modules.

Open-source licensing does not itself guarantee freedom from third-party
patent, trademark, copyright, dataset, model or other
intellectual-property rights. Each dependency and deployment requires
appropriate review.

## Disclaimer

**jfxlms / OpenTwin AI Learning Management & Digital Education Platform
is a research, educational and engineering project.**

AI-generated tutoring, feedback, assessment suggestions and analytics
can be incomplete or inaccurate. High-impact educational decisions
should use appropriate human review and institutional governance.

Deployments involving minors require particular attention to
age-appropriate design, privacy, security, safeguarding and applicable
legal requirements.

The BID repository template is used solely as a
**documentation-structure reference**. jfxlms does not claim BID/IDB
funding, sponsorship, endorsement, catalog membership or institutional
affiliation.

## License

The actual jfxlms project license should remain in the repository root
as `LICENSE`, `LICENSE.md`, or its existing equivalent.

Third-party libraries, LMS platforms, datasets, models, standards
implementations, course materials and documentation retain their
respective licenses and terms.

Do not automatically apply BID/IDB institutional licensing language,
copyright notices, funding statements or disclaimers merely because its
documentation template informed this README.

------------------------------------------------------------------------

## OpenTwin Learning Principles

**Open Architecture · Adaptive Education · Interoperability · Modular
Digital Twins · Human Oversight · Privacy by Design · Accessibility ·
Provenance · Reproducibility**

> Open learning infrastructure without mandatory vendor lock-in.\
> Educational digital twins based on transparent, governed evidence.\
> AI as a tutor and assistant, not an unquestionable authority.\
> Interoperable learning services through documented interfaces.\
> Reusable educational resources and independently replaceable
> components.\
> Systems engineering from architecture through simulation and
> verification.
