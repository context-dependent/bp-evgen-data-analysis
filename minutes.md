Meeting Minutes
================

## Working Meeting 3

[2022-11-13](.aside)

Working Meeting 3

### Attendees:

- Max, Thomas

### Context:

- we planned to have this meeting after chatting ab it about the
  conversations that Vibha, Tanya, Sandra, and I have had

### Intentions:

- Agree on the Scheme of things we need
- Prioritize and discuss

### Content

- Things I think we need:
  - Concept of a data analysis project, adn that concept needs to be
    both used and useful. It needs language, expectations, and
    procedures.
    - Definitions
    - Procedures
      - Inputs, Outputs
      - Expectations
      - Instructions
  - Tooling to support the obligations outlined by the DAP concept
  - Skills development programme, to let the uninitiated participate in
    the new DAP concept
  - Collective intelligence procedures and tooling.
    - Difficult? Yes. How to get people to participate?
- What are Expectations?
  - Conditions that inform decision-making about resourcing and review
  - e.g. it should take roughly x hours to complete y task
- Start with Definitions, then move to Expectations, Instructions
- How to calibrate specificity?
  - Max’s idea is that more specifity makes it easier to interact with,
    or like do as a neophyte
  - Be specific as we can be, be specific about unspecificity
- Story mapping:
  - How do you set up your inputs to support effective data analysis?
    - The key for setting up inputs to be effective is ensuring the
      predictability of working with inputs
    - Analysis plan should be one thing, that reflects both current and
      historical understandings of the approach

``` mermaid
graph LR
  A[AP0 Pre-contract] --> B[API Pre-data]
  B --> |per reporting cycle| C[APII Post-data]
  C --> Y(Exploration Log...? Analysis Report?)
  Y --> X[APIII Outputs]
  B --> D[Data collection scheme]
  B --> J[Objectives and Methods]
  D --> E[Surveys]
  D --> F[Non-Survey Instruments]
  D --> G[Linkage Details]
  D -.- H(Toy Datasets)
  H -.- I(Example Functions)
  H --> J
  J --> D
  K(Org Standards) --> L(Linkage hygeine)
  K --> M(Scale validation)
  K --> N(Sample Size)
  C --> O(Explore)
  O --> P(Discuss)
  P --> Q(Reconcile)
  Q --> R(Ideate)
  R --> S(Revise APII)
  S --> O
```

- What’s an example example function?
  - Say we have an evaluation with surveys W, M, V, and Salesforce
    database E
  - Given generated datasets W\* … E\*,
  - We could make an example function for calcualting pre-post changes
    in key metrics

<!-- -->

    function calc_pre_post_key_metrics(W, M, V, E)
      join the data,
      identify pre-post
      aggregate

- How easy is it to make a toy dataset?
  - Trivial, so long as you’ve thought through and aligned on what’s
    being represented and how
- Why have toy datasets and e.g. functionality?
  - by comparison, will clarify violations of expectations in the actual
    data
  - forces very concrete reasoning about the analysis approach early in
    the planning process (while everyone’s still on the project)
  - has upside for collective intelligence, code sharing and review,
    etc.
- How does the APII loop operate in situations with multiple reporting
  cycles?
  - If you have an interim report I and final report F,
  - and I is answering questions \[A, B, C\], F is answering questions
    \[A, B, C, D, E\]
  - then the APII loop for F is abbreviated to the extent that you
    figured out how to answer questions \[A, B, C\]
- What does a reporting cycle look like?
  - Start with APII
  - Once you have APII, how to get to outputs?
    - Categories of outputs
  - Would be nice to come out of APII with a clear idea of what to
    produce
- What questions remain?
  - This process map deserves a view with fresh eyes next week
  - Max wants to get the Coalition of the Willing together on this
  - We need definitions, and a product
  - Who and where to test

## Working Meeting 4: Governance and Planning

<div class="column-margin">

Date: 2022-11-17 Chair: Max Scribe: Thomas Other: Vibha, Tanya

</div>

Max booked this meeting to run through the conversation between the two
of us last week in view of Tanya and Vibha, and then to outline the
governance and direction of next steps.

### Content

- Overview of the skeleton
- Everyone is down with the concept, or at least the intention
- MP: Say TM and I keep pushing toward an MVP, what do we want in terms
  of people and things?
  - Who makes sense?
    - VM: Sandra, all agreed!
    - TS: Should keep the group small, “bounded”. Maybe anyone at a
      relatively senior level that has some oversight function for data
      analysis. Engagement leads should have input at some point.

<div>

> **Teams**
>
> |            **Role** | Team                              |
> |--------------------:|:----------------------------------|
> | *Development Leads* | Thomas, Max, Vibha                |
> |          *Steering* | Vibha, Tanya, Sandra, Thomas, Max |
> |             *Input* | Engagement Leads                  |

</div>

- Overall roadmap:
  - MP + TM design high-level product touchstone
  - Steering meets to design and assign projects
- Start small and slowly, incremental progress needed
- VM: Just remembered, maybe Data Solutions should be involved, Sandra
  has flagged issues
- Involve DS later in the process
