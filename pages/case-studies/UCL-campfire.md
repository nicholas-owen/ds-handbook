---
# ============================================================================
# Case study (campfire) template
# Copy this file into pages/case-studies/<your-case>.md and fill it in.
# Required fields are marked (mandatory). Everything else is optional but
# encouraged – the more you fill in, the more useful the case is to others.
#
# Some fields use a controlled vocabulary – you set a key, and the layout
# looks up the human-readable label from a YAML in _data/case_study/.
# If you need a value that isn't there, propose it in your PR rather than
# inventing one inline (so filtering and counts stay consistent).
# ============================================================================

title: " UCL - Data Steward as a profession - WIP"          # mandatory – short, specific
layout: case-study                 # mandatory – leave as-is
type: [Case Study]                 # mandatory – leave as-is
search_exclude: true               # remove this line when ready to publish

# 20–30 words. Used in meta tags, search results, and the highlights box at
# the top of the page. Easier to write last, once the rest of the page exists.
description: How UCL built a team of 19 research data stewards within its Advanced Research Computing department, using a research-technology professional job family model funded through research and core income.

contributors: [Nicholas Owen, Ines Chaves, Robert Andrews]          # mandatory – names must match _data/CONTRIBUTORS.yaml
page_id: ucl-data-steward-profession      # mandatory – lowercase, hyphenated

# ---------------------------------------------------------------------------
# Context card – populates the at-a-glance box at the top of the page.
# Fields tagged [vocab] use a key from _data/case_study/<file>.yml.
# Fields tagged [free] are typed verbatim by you.
# ---------------------------------------------------------------------------

lead_org: "UCL (ELIXIR-UK)"       # [free] main org behind the work
country: UK                        # [vocab] countries.yml – 2-letter key
# If your ELIXIR node matters, mention it inside lead_org – e.g. "CSC (ELIXIR-FI)".

partners:                          # [free] optional – vendors, universities, funders
  - "ELIXIR-UK"
  - "ELIXIR Europe"
  - "Global Alliance for Genomics and Health (GA4GH)"
  - "BioFAIR"
  - "Research Data Alliance (RDA)"

# Pick the right size of the work.
# individual | team | institutional | national | international
scale: institutional               # [vocab] scales.yml

# Pick the discipline the work ORIGINATED in, not who could adapt it later.
# life-sciences | physical-sciences | humanities | cross-domain | domain-agnostic
domain: life-sciences              # [vocab] domains.yml

# One or more – pick the PROBLEMS this case addresses, not the solution.
# Full list in themes.yml: training-gap, unclear-roles, policy-gap,
# tooling-gap, sustainability, legal-compliance, stakeholder-engagement,
# community-building.
themes:                            # [vocab] themes.yml
  - unclear-roles
  - tooling-gap
  - stakeholder-engagement
  - community-building
  - sustainability
  - training-gap

start: 2022                        # [free] year the work began

# Lifecycle of the work today.
# active | evolved | paused | archived
status: active                     # [vocab] outcome_status.yml

# Optional link to the official activity / project page outside this
# handbook (the institutional page, the funder page, the project site).
# Renders as a "Visit the activity page" link inside the context card.
# Override the link text with `external_url_label` if you need to.
external_url: https://www.ucl.ac.uk/advanced-research-computing
external_url_label: UCL Advanced Research Computing

# ---------------------------------------------------------------------------
# Lead quote – one sentence you wish someone had told you at the start.
# Renders as a pull-quote near the top. Skip if you can't think of one.
# ---------------------------------------------------------------------------
lead_quote: "It's the common purpose that defines research data stewardship better than the particular skills involved."

# ---------------------------------------------------------------------------
# Cross-references (optional but encouraged) – page_ids of related guidance
# pages and maturity indicators. Both render as a "Related" block at the
# bottom of the page.
# ---------------------------------------------------------------------------
# Cross-references – rendered as a "Related pages" block at the bottom.
# Nested by type; each section becomes a row of slim tone-aware tiles.
# Type keys recognised: Guidance, Case_Study, Maturity_Indicator.
related_pages:
  Guidance:
    - g-writing-rdm-strategy
  Case_Study:
    - other-case-shortname
  Maturity_Indicator:
    - mm-strategy-defined

# ---------------------------------------------------------------------------
# Resources – render as ELITMA-style tables (Templates / Internal /
# External) at the end of the page. Two ways to add an entry:
#
# 1. Reference an ID from _data/tool_and_resource_list.yml (preferred
#    for shared resources like RDMkit, FAIR Cookbook, DSW…):
#
#        resources: [rdmkit, fair-cookbook, ssi]
#
# 2. Add an inline entry for one-off resources unique to this case study
#    (the SOP, the grant reference, the institutional URL):
#
#        - name: "Resource title"
#          url: https://example.org/resource
#          description: One-line context.
#          category: external_resource   # or template, internal_resource
#
# Both forms can be mixed in the same list.
# ---------------------------------------------------------------------------
resources:
  - name: "FAIR Data Principles (2016)"
    url: https://www.go-fair.org/fair-principles/
    description: The foundational principles guiding UCL's data stewardship approach — making data Findable, Accessible, Interoperable, and Reusable.
  - name: "Realising the European Open Science Cloud (2016)"
    url: https://ec.europa.eu/research/openscience/pdf/realising_the_european_open_science_cloud_2016.pdf
    description: EU High Level Expert Group report that emphasised the importance of data stewardship and estimated a need for over half a million 'core data experts' within a decade.
  - name: "ARC Life Sciences Collaborations"
    url: https://www.ucl.ac.uk/advanced-research-computing/collaborations-consultancy/life-sciences-collaborations
    description: ARC's dedicated Life Sciences theme group, led by Nicholas Owen, providing domain-specialist data stewardship and computational support to UCL life science researchers.
  - name: "ELIXIR-UK"
    url: https://elixiruknode.org/
    description: The UK node of ELIXIR, supporting training, tools, and data resources for life sciences research data management; a key external community for UCL's life sciences data stewards.
  - name: "ELIXIR Europe"
    url: https://elixir-europe.org/
    description: Pan-European infrastructure for biological information, providing standards and community frameworks that inform UCL's FAIR data practice in life sciences.
  - name: "Global Alliance for Genomics and Health (GA4GH)"
    url: https://www.ga4gh.org/
    description: International standards body for responsible genomic and health data sharing; standards developed through GA4GH inform UCL's genomics data stewardship workflows.
  - name: "BioFAIR"
    url: https://biofair.uk/
    description: UK national research infrastructure for FAIR life sciences data, providing a community and technical framework that complements ARC's institutional data stewardship work.
---


## Why this case (mandatory)

>Note: What problem or gap did this work address, and why was it worth doing?
>Set up enough institutional context that a reader from a different
>country or sector can follow.
>
>- What was the situation before?
>- Who was affected (researchers, stewards, leadership)?
>- Why now – what made this the moment to act?
>
>Two or three short paragraphs. Don't recite policy – tell the story of
>the gap. Concrete details (sizes, dates, the specific incident that
>triggered it) help more than abstractions.


UCL's research data function began as a conventional research IT services team sitting within a large Information Services division. In 2016 — the year the FAIR Data Principles were published and the EU High Level Expert Group report *Realising the European Open Science Cloud* highlighted the need for hundreds of thousands of "core data experts" — the team was primarily occupied with managing research data storage and implementing an institutional data repository. The concept of a named "research data steward" role did not exist at UCL, and few people anywhere had yet heard the term.

The gap was not just one of vocabulary. The team's model was transactional and services-led: researchers pressed buttons, submitted forms, and received outputs. Direct collaboration with researchers on the substance of their data management was limited. There were no mechanisms to intervene in the actual research process, no structured metadata capture, and no community connecting people across the university who were already doing data stewardship work without calling it that.

The moment to act came in 2022, when the team was reorganised and rebranded as the Centre for Advanced Research Computing (ARC). This restructure created the conditions — institutional identity, a new funding model, and a formalised job family framework — that made building a professional data stewardship team possible.



## What we did (mandatory)

>Note: The actual approach. Walk through what you tried, in roughly the order
>you tried it. Bring people and tools in as they appear – no need for a
>separate "stakeholders" or "tools" section.
>
>- What was the first move?
>- Which tools, frameworks, or existing resources did you use? (e.g.
>  RDMkit pages, DSW templates, internal SOPs, the FAIR Cookbook)
>- How were researchers / leadership / partners engaged at each step?
>- Was this brand-new, or built on something existing?
>- Roughly how much effort was involved (FTE, calendar time)?
>
>Be concrete. *"We held a 30-minute intake call with the PI before each
>new project"* beats *"We instituted a stakeholder-engagement protocol"*.
>If you got something wrong and pivoted, say so here – the pivot is part
>of the story.

The foundation for everything that followed was the creation of a **research technology professional job family** framework within ARC. Rather than hiring individuals into one-off, bespoke roles, the department defined five job families: Research Software Engineers, Research Infrastructure Developers, Research Data Stewards, Research Data Scientists, and PRISMs (Professional Research Investment and Strategy Managers). Every member of ARC belongs to one of these families. This structure had three practical consequences:

First, it removed the friction of recruitment. Generic job descriptions mean HR do not need to review and approve from scratch each time a post is created, cutting what had previously been a four-month approval cycle. Job adverts are then tailored within the generic framework to attract the specific skills needed at any given time.

Second, it created career pathways. Before the restructure, the only promotion route for a technical specialist was into management. The job family model allows progression within each profession, which matters particularly for retaining experienced people.

Third, and most significantly for sustainability, it enabled **permanent contracts**. Many of the team's recruits had come from departmental research roles, often postdoc positions, characterised by short-term contracts and job insecurity. ARC's model, funded substantially through research income written into grant bids, provides enough ongoing flow of projects that individuals can move between them without returning to precarity. As word has spread, this stability has itself become a recruitment advantage.

The **funding model** was built on the precedent set by UCL's Research Software Engineering team, which has operated since around 2013 and achieved self-sustainability through research income. UCL negotiated that grant income, including overheads (as UKRI guidance now officially supports), can be used to grow the department rather than purely to deliver project outputs. Research technology professionals are written into bids wherever possible. Bringing in overheads allows the team to maintain and develop core services alongside project work.

The **team composition** was intentionally broad. The data stewards team includes people from technical data librarianship, university administration, data science, academic publishing, clinical trials, specialist scientific equipment (e.g. imaging), and departmental research backgrounds. Some are domain specialists, including life science expertise relevant to the ELIXIR community, and some are generalists able to support services across disciplines. The team operates a hybrid model: everyone is expected to engage with both the services side and the research side of the work, so that service design is informed by direct research experience and researchers receive relevant signposting to institutional services.

Alongside the core data stewards team, ARC organises its collaborative work into **domain-specific research theme groups** that give researchers a more direct point of contact with specialists who understand their field. The **Life Sciences theme group**, led by Nicholas Owen, is the most directly relevant to the ELIXIR community. The group brings together Research Technology Professionals with dual fluency in life sciences research and computational methods. Their work spans omics pipelines (genomics, transcriptomics, epigenetics using tools such as Nextflow), bio-image analysis (napari, FIJI, large imaging datasets), standards in computational biology (COMBINE, BioModels, BioSimulators, Open Source Brain), and neuroscience informatics. Critically, applying FAIR data principles to life sciences outputs is named explicitly as a core commitment of the group — bridging the abstract principles of the wider data stewardship team to the concrete workflows of bench and computational researchers. The group also runs a dedicated teaching series at UCL's Division of Biosciences, covering reproducibility, data management, HPC, and AI, an example of stewardship being enacted through capacity-building rather than purely through direct service delivery. Other ARC theme groups cover Healthcare, Medical Imaging, High Performance Computing, Trusted Research Environments, and DevOps/cloud, meaning that a researcher in almost any domain can engage with specialists who recognise their context, while drawing on the shared infrastructure and governance of the central team.

**External community engagement** has been an active and deliberate part of how the team builds credibility, stays current, and contributes back to the broader profession. UCL's life sciences data stewards are engaged with **ELIXIR-UK** (the UK node) and **ELIXIR Europe**, the pan-European infrastructure for biological information. This engagement shapes how UCL implements FAIR data practice in life sciences, drawing on ELIXIR's training frameworks, tool registries, and community standards rather than building from scratch, and in turn contributing UCL's experience back to those communities. The team is also connected to **GA4GH** (Global Alliance for Genomics and Health), the international standards body for responsible genomic and health data sharing, whose standards inform UCL's genomics data stewardship workflows. **BioFAIR**, the UK national research infrastructure for FAIR life sciences data, provides a further community and technical framework that complements ARC's institutional work and situates it within a national landscape. These engagements are not peripheral, they are part of how a central institutional team remains relevant to specialist researchers who could otherwise view generic data stewardship support as too distant from their actual practice.

Beyond the core team, ARC ran **community of practice workshops** to identify and connect people elsewhere at UCL who were doing data stewardship work without the label. Participants placed sticky notes on a research data management lifecycle wheel to indicate where their work fell. This brought in colleagues from across all background at UCL, as well as departmental research staff not yet connected to any broader network.

The **services portfolio** grew in parallel with the team. Starting from research data storage, it expanded to include: an institutional data repository (launched 2019, based on Figshare), an electronic research notebook service based upon RSpace, Globus for large-scale data transfer, a data safe haven (being modernised into more flexible Trusted Research Environments), and a managed third-party data service to reduce duplication across the university. HPC infrastructure was integrated more closely with research data storage.


## What changed (encouraged)

>Note: What's different now? Concrete outputs are most useful – a training
>course delivered, a workflow adopted, a policy written, a tool deployed,
>a number that moved.
>
>- What was produced or implemented?
>- What's the evidence it worked? (uptake numbers, feedback, metrics,
>  anecdotes – all valid; pick what you actually have.)
>- What barriers came up, and which factors helped you push through?
>  (Leadership backing, an existing community, a deadline, a champion?)
>
>If the work hasn't produced visible change yet, say so – *"too early to
>tell, will revisit in 12 months"* is a fine answer when it's honest.
>Better than reaching for impact that isn't there.

UCL went from having no named research data stewards in 2016 to a team of 19 at the time of writing. The department as a whole grew from approximately 40 people as Research IT Services to around 140 in ARC.

The shift from transactional to collaborative working is the qualitative change the team points to most directly. Stewards now intervene in active research processes, helping researchers enact the data management plans they have written, rather than simply receiving deposits at the end of a project. This is described as the difference between data management being described as good practice and it actually taking place.

The community of practice initiative identified data stewardship activity distributed across UCL that had previously operated in isolation, bringing those practitioners into a shared network.

Permanent contracts have enabled knowledge retention. Previously, when researchers on short-term contracts moved on, institutional knowledge left with them. That pattern has been disrupted.

UCL is now described (at time of writing) as appearing at the top of Google searches for UK universities doing research data stewardship, an informal indicator of visible leadership in the field.

The Life Sciences theme group has made ARC's stewardship offer tangible for one of UCL's largest research communities. Domain-specialist stewards working alongside bench and computational researchers — on omics pipelines, imaging data, and computational biology standards, represent a qualitative shift from the earlier model in which researchers had to translate their specific data challenges into generic service requests. Embedding FAIR principles within active research workflows, rather than at the point of data deposit, is the practical manifestation of the team's ambition. The group's teaching series at the Division of Biosciences marks ARC's stewardship extending into researcher capacity-building at the faculty level.

External engagement with ELIXIR-UK, ELIXIR Europe, GA4GH, and BioFAIR has given UCL's stewards a visible presence in the communities that matter most to life sciences researchers. This external positioning helps with internal credibility: researchers are more likely to trust and engage with stewards who are known contributors to the standards bodies and communities those researchers already rely on. It also keeps the team embedded in evolving best practice rather than at risk of institutional insularity.



## What we'd tell others (mandatory)

>Note: The lesson, the caveats, the conditions for replication, and what
>happens next – bundled because they overlap in practice.
>
>- **What worked, and why.** The one or two things you'd repeat without
>  hesitation if you were starting over.
>- **What didn't work, and how you adapted.** The corner you painted
>  yourself into. Future contributors learn most from these.
>- **Transferability and scaling potential.** Can this approach be reused
>  by another institution or individual? What conditions are required
>  (leadership buy-in, existing service, specific funding, a particular
>  legal context)? What adaptations might be needed? Be honest about
>  what was special about your setting.
>- **Sustainability and next steps.** How is the work currently supported
>  or funded? Who maintains or owns it? What are the plans for
>  continuation, embedding, or scaling? If continuity is uncertain, say
>  so.

**What worked, and why.**

The single most transferable element is the job family framework. Defining the profession before recruiting into it, rather than creating individual posts reactively, solved multiple problems simultaneously: HR friction, career progression, recruitment attraction, and the ability to offer permanent contracts. The precedent of an existing, successful job family (Research Software Engineers) was essential in persuading institutional gatekeepers that the model was credible. If your institution has an established RSE team, that is the argument to make.

Funding through research income rather than purely through core institutional budget is what enabled growth. Getting research technology professionals written into grant bids is achievable; UKRI guidance now explicitly supports including overheads. The initial persuasion of research teams to include these costs is the hurdle, and it requires demonstrating value in practice first.

Organising collaborative work into **domain-specific research theme groups** has been important for researcher engagement. A central data stewardship team risks being perceived as too generic to help with specialist research data challenges. Having an organised Life Sciences theme, with stewards who know bioinformatics, who understand ATAC-seq, who are active in ELIXIR and GA4GH — removes that barrier. Researchers engage with people who speak their language. The theme groups do not fragment the team; they are a front-door for domain-specific entry points that feed into shared infrastructure, governance, and professional development. Other institutions building stewardship teams should consider how they will make the offer legible to specialist research communities, not just to research support staff.


**What didn't work, and how you adapted.**

Generic job descriptions while essential for speed and HR efficiency sometimes advertise such a broad range of skills that they may deter applicants. The team is aware of this and continues to work on how the profession is described and communicated. The balance between services work and research involvement also remains a live tension: currently we acknowledge a drift toward the research side that left services somewhat under-supported. We continue to balance cost recovery from research projects and service management. Services are harder to fund through grants, which creates a structural pull toward research-facing work that requires active management.

Earlier iterations of the team were too siloed from other teams due to project load. Collaboration across research technology professions, not just between stewards and researchers, is essential, and the tighter integration of research data storage and compute infrastructure reflects that lesson learnt.


**Transferability and scaling potential.**


**Sustainability and next steps.**
The team is funded through a combination of core departmental budget and research income. Permanent contracts depend on a continuing flow of projects, which has held so far but requires ongoing effort to maintain. Long-term technical goals include automated metadata population from services, provenance capture throughout the research lifecycle, and expanded trusted research environments for sensitive data — all of which represent future capacity requirements. The work with ELIXIR and BioFAIR through the Pathfinder project will one of the many vehicles through which UCL works to embed the profession more formally at all levels.

External community engagement — with ELIXIR-UK, ELIXIR Europe, GA4GH, and BioFAIR — is not simply a reputational activity; it is part of how the team sustains its relevance and influence. Contributing to standards development and community training means that UCL's practices stay aligned with what the broader research community expects, and it means that stewards bring back knowledge and connections that strengthen the institutional offer. For other institutions, engaging with these communities early — before a full team exists — is a practical way to build credibility and find collaborators. Broader national community of practice development (along lines seen in Ireland, Canada, and Austria) is identified as a gap in the UK that the team is keen to help address through these channels.


<!--
  Don't add a `## Resources` heading here – the layout renders the
  `resources:` frontmatter list automatically as a table at the bottom
  of the page.
-->
