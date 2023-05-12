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

## Working Meeting 5: A Hypothetical

- Thomas, Max
- Build a hypothetical program, around which we can develop a platonic
  dataset / workflow
- Extend the description of FairWeather

### Burning Questions?

- What kinds of situations do we want the passenger to be confronted
  with?
  - Start with a list and then ask people
  - List all in the output, and rationalize their treatment.
- Is it an evaluation?
  - Yeah, for now!

### Situations

- Research questions as stated are not answerable in the data
  - sometimes there is an ill-defined question
  - sometimes there is a well-defined question that cannot be answered
- Lack of clarity wrt about whom the analysis cares
- Missing data
- Joint Pain
  - Longitudinal chaos
  - Cross-sectional linkage issues
- Sample size and representativeness\*
- Tech heck (API struggles)
- Client conflict!!(how to explain)

### Sample size

- What are we representing?
  1.  for our typical audience, representativeness starts with
      representing the program participants

  - When we have high missingness, what does a result *mean* about the
    program participants.
    - there’s sampling error
    - There’s nonsampling error as well, driven by nonresponse bias
  - Guidance on how to treat it, how to talk about it. How to defuse the
    incorrect assumptions your readers might have.

  2.  also leans into representing the general population of people who
      might take the program were it scaled up.

  - Coming up with a stock blurb that says “these results aren’t
    representative of the broader population”
  - The question is “Should we be doing this in the future?”
    - If you’re running a pilot with 30 people what do you expect? - Max
      Palamar
    - If you’ve got 200 people, ok, now we’re talking
  - Benchmarks?

### What does the simplest viable example program have?

- A really textbook EAS / EO program
- You can come up with a dumb question
- Tiers of services to introduce complexity
- Some admin data that doesn’t correspond exactly to survey data
- Several surveys, some of which have low response rates
- Several questions on individual surveys with low response rates.

### What does the program look like?

- Intake
- Resume help
- Streaming
  - Supportive / longer term JMPI+ (Manitoba worksish?)
  - JMPI
  - No JMPI

### What datasets do we have?

- CAMSish
- Baseline, Exit, Follow-up
- Service provider jank (a word document, or a junky excel sheet, or a
  series of pdf forms)
  - microdata is the most frequent, mirrors supplementary ‘needs
    assessment’-style data collection
- Some cost figures or w/e

### Name ideas

- Furious Max’s The Jobagon
- Job Predator
- Jobinator
- The Book of Jobs

### Research Questions

- Who does this program reach? (could be bad or good, depending on the
  defn’ of target pop)
- Satisfaction?
- Employment outcomes?
- Confidence, happiness, soft skills? (something quanty, but one
  plausible and one unlikely)
- Does JMPI+ produce sustainable employment outcomes?
- Does JMPI+ do better?
- Is JMPI+ worth it?
- Inter-group differences? (this could be bad, and like… get good?)

### Client Context

- Piloting JMPI+, a new service offering
- Funder has mandated evaluation
- They’ve subcontracted us to be the evaluator
- The Jobagon has a mandate to serve unemployed people in general
- JMPI+ is aimed specifically at people on social assistance, per funder
  targets
- The Jobagon serves 2000 people per year

### Targets

- 300 participants (permits much, forbids some) in JMPI+
  - 240 of whom are on social assistance
  - 150 of whom belong to one or more hdes groups
- 90% CAMs-style satisfaction
- 80% Placement rate
- 70% Employment rate at follow-up

### Miscellany

- Baseline survey collected before enrollment into JMPI+, but Exit and
  Follow-up are only administered to JMPI+ers

### Where are we at

- The scene is set
- Time to make the datasets

## Working Meeting 6: Overall Process revisit

- Where are we starting?
  - More work needed to get to MVP on overall process

### Refined Stages

**Bolded** items are clear hooks for tools, rules, standards.

`AP[X]` is the Xth analysis planning stage `R[X]` is the Xth artefact of
the analysis process

1.  Pre-contract

- Proposal
- Research objectives
- `AP0`: **Preliminary plan**
  - `R0`: **High-level methodology**

2.  Data design

- Survey designs
- Admin datasets
- `AP1`: **Specify approach**
  - `R1`: **Detailed methodology**
  - `R2`: **Input data dictionary**

3.  Data collection

- Monitoring:
  - `R3`: **Monitoring log**

4.  Analyze

- Have the data for the analysis
- Have accumulated insights
- Have monitoring logs
- Explore loop:
  - `R4`: **Exploratory output pile**
  - `R5`: **Decision log**
- `AP2`: revisit `R1`: **Detailed methodology**
  - Realign analysis objectives with project objectives
  - Assess feasibility through exploration
  - Identify limitations and enumerate implications
  - Justify methodological adapatations
  - Iteratively build `R6`: **data pipeline**
  - Document final data pipeline
  - Finalize methodology

5.  Publish

- `AP3`: **Schedule of deliverable outputs**
  - `R7`: **Analysis outputs**
