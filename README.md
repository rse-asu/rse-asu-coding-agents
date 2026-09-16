# Resources on Coding Agents and Scientific Computing

It may be useful to both make resources available to the public community, as well as allow for the collection of suggested new resources. Over time we could decide how to integrate this list into a public project.

This list was initially compiled by Peter Dresslar in September, 2026.

## Resource Categories

The resources suggested below are machine-formatted and human-annotated.

### Perspectives on coding agents in research computing

- [Who is scientific code for? Maintaining human-readable landmarks in agent-written code](https://arxiv.org/abs/2607.25975) — Elle O'Brien (July 2026; workshop position-paper preprint). Your human reviewer thinks this is a great paper on the topic and very aligned with the "challenges" we discussed recently. Quote: "Storey [9] has recently proposed that agent-involved software work accelerates the accumulation of cognitive debt... and intent debt...  I’m seeing fascinating responses... **That means intent is being captured through customs that are never made explicit or shared**, and this may be quietly making scientific software infrastructure less amenable for collaboration and reuse." Brilliant. Read this one.

- [Skills are infrastructure, and a new open-source artifact class](https://ospo.gwu.edu/skills-are-infrastructure-and-new-open-source-artifact-class) — Lorena A. Barba (August 2026; GW Open Source Program Office essay). Barba draws on hands-on work with agents in research and teaching to argue that skills are shared infrastructure: packaged expertise that needs review, provenance, licensing, and maintenance. The examples run from scientific writing to numerical stability checks and research budgets. Very relevant to RSEs, especially the warning that a "beautifully organized skill" can still encode a bad scientific protocol. See also the preprint, [Reproducibility in the Age of Agentic AI](https://arxiv.org/html/2609.11728v1).

- [The human experience of coding with an agent](https://matsen.fredhutch.org/general/2025/11/07/human-experience-with-agents.html) — Erick Matsen (November 2025; personal reflection). A scientist's personal account of attention, working habits, and learning while using coding agents, including questions about how future scientists develop expertise. Quote: "If industry gets to use AI to develop apps that keep people glued to their smartphones, I want to be able to use it to advance science."

- [Research Software Engineers in the Age of GenAI: Same Value, Changing Practice](https://www.researchsoft.org/blog/2026-05-28/) — Stephan Druskat and colleagues, Research Software Alliance (May 2026; workshop perspective). Necessarily drier than O'Brien and Matsen--this is a work by committee--but there are a couple of terrific and possibly reusable illustrations about the need for RSE involvement to evolve.

- [Position Statement on Generative AI in the RSE Workplace](https://github.com/Academic-Data-Science-Alliance/rse-ai-position-statement/blob/main/RSE-AI-Final_Statement.md) — ADSA and US-RSE (community position statement). A cautious position on AI in the RSE workplace. Useful observations in particular about "RSEs are well positioned to close knowledge gaps," putting a finer point on the ReSA reference above.

### Existing studies and surveys

- [How Scientists Use Large Language Models to Program](https://arxiv.org/abs/2502.17348) — Gabrielle O'Brien (April 2025; peer-reviewed CHI study). IRB-empowered scientific inquiry, with a large survey of 199 scientists at one university, followed by 14 interviews and examination of interaction logs. Naturally, Feb 2025 was a relatively early publication date for this work; coding agents are materially different in late 2026. Nonetheless the methodology in particular is instructive.

- [A survey of generative AI adoption and perceived productivity among scientists who program](https://arxiv.org/abs/2512.19644) — Gabrielle O'Brien and colleagues (December 2025, revised April 2026; survey preprint). Follow-on survey. 868 scientific programmers in summer 2025 (still early!) on tool choices, coding practices, perceived productivity, and reasons for non-use. Students, not surprisingly, reported greater felicity toward coding agents--note, though, that we have references above from which we could infer that students are the least likely to truly benefit.

- [Coding agents in the social sciences](https://www.anthropic.com/research/coding-agents-social-sciences) — Thomas Lyttelton and colleagues (May 2026; survey report published by Anthropic). This is an Anthropic study, so caveats may apply. On the other hand, the data reported are some of the most comprehensive available. The survey hits 1260 quantitative social scientists in February–March 2026; with 20 percent reporting CA usage. Self-reporting study methodology; and, critically, no empirical gains established.

- [AI Coding Agents in Social Science: Methodologically Diverse, Empirically Consistent, Interpretively Vulnerable](https://arxiv.org/abs/2606.11456) — Meysam Alizadeh and colleagues (June 2026; experimental preprint). From the abstract: "The deployment of LLM-based agents in scientific analysis raises opposing concerns: that agents may reduce methodological diversity, or that they may amplify the analytic flexibility through which researchers reach motivated conclusions." Very in-line with some of the experiences I shared recently, and the results confirm real dangers to science due to, effectively *social* problems between agents and humans. **Read this one! Makes a strong case for RSE assistance. Plenty more investigation to do along these lines too!**

- [Scientific computing in the age of agentic AI: an exploratory field report](https://doi.org/10.64898/2026.07.29.741496) — Jeremy Li and colleagues (2026; exploratory preprint with OpenAI-affiliated authors). Eight terrific, deep, contributor-written case studies, mainly in the life sciences. Describes engineering assistance alongside persistent scientific validation and maintenance challenges. Not a lot of empirical conclusion but the use cases are worth the price of admission. Points to a well-detailed reference implementation: [MHCflurry](https://github.com/openvax/mhcflurry), an OpenVax (immunology; established research software) project.

- [SWE-bench Science: Can Coding Agents Resolve Engineering Tasks in Science?](https://arxiv.org/abs/2608.19799) — Zhipeng Xu and colleagues (August 2026, revised September 2026; benchmark preprint). Our newest entry introduces a benchmark that may or may not be useful; however, there are many referenced projects--and, most importantly, this reference serves to remind that the effects of coding agents in science are global, not local to one country.

### Practices, validation, and reproducibility

- [Twelve quick tips for AI-assisted coding in science](https://doi.org/10.1371/journal.pcbi.1014428) — Eric W. Bridgeford and colleagues (July 2026; PLOS Computational Biology education article). These tips are generally helpful, though stuck in a text article (a companion website might be nice); different users will necessarily find different takeaways. I like the discussion of software testing with coding agents in particular.

- [Writing scientific code using agents](https://matsen.fredhutch.org/general/2025/11/04/scientific-coding-with-agents.html) — Erick Matsen (November 2025; practitioner guide). A more personal but possibly more practical guide than the one in the PLOS article. Excerpt: "**No Silent Fallbacks**: Code must fail immediately when expected conditions aren't met. Silent fallback behavior masks bugs and creates unpredictable systems." So important! AI tends to get this wrong as it is likely rewarded to aim for fault-tolerance.

- [AI Coding Tools at NERSC](https://docs.nersc.gov/development/coding-agents/) — NERSC (practical HPC guide; accessed September 2026). Examples for supplying logs and environment details, requesting small changes, checking scheduler settings, and validating results before larger runs. Includes reusable project instructions for agents. The commands and operating guidance are specific to NERSC's Perlmutter system and need adaptation for other clusters. GPT Astra annotated this one; your human author cannot do a better job in this case.

- [Agentic AI-Assisted Coding Offers a Unique Opportunity to Instill Epistemic Grounding during Software Development](https://www.nist.gov/publications/agentic-ai-assisted-coding-offers-unique-opportunity-instill-epistemic-grounding-during) — Magnus Palmblad, Jared M. Ragland, and Benjamin A. Neely (July 2026; Journal of Proteome Research letter). Proposes community-maintained `GROUNDING.md` files that encode scientific validity requirements and conventions for coding agents, using proteomics as an example. Inclusion here is not a validation of the specifics, but very much so an endorsement of the ideas leading up to the specifics.

### Example projects

- [Pedro H. C. Sant'Anna of Emory U.](https://github.com/pedrohcgs/claude-code-my-workflow) has a "A ready-to-fork Claude Code template for academics using LaTeX/Beamer + R. Multi-agent review, quality gates, adversarial QA, and replication protocols" from an econometrics prof. There are several interesting concepts here, though I wonder if the total package would suit a large percentage of other researchers. (Fork, or imitate? might be a question.) Still, the LaTeX tooling is genuinely exciting, and the `explorations` directory is a great idea for handling noodling.

- [Honey Bee Behavior](https://github.com/Collective-Logic-Lab/honey-bee-behavior) and [Honeybee Hive Video](https://github.com/Collective-Logic-Lab/honeybee-hive-video) — Two connected group projects I am personally involved in at the Collective Logic Lab. Very different goals mean very different approaches to AI coding agents (and AI in general). The Honey Bee Behavior project has a number of student notebooks and is for almost pure exploration. Here, we want to keep coding agents largely out of modifying code, especially the noodling through scientific understanding of the subject bees. A small `src` directory, where the finished code accretes, may be updated on a limited basis with agents. The Honeybee Hive Video repo is fully agent-integrated, and here the challenges are far different--and so the setup with agent communication attempts to reflect this. We will continue to seek best practices in both cases.

### Coding agent tooling for science

These extend coding agents with scientific instructions, data access, or connections to analysis environments. Disclaimer: Have not tested all of these; listing them as examples of what exists. This list could be widely expanded, and it would be good to get more testing on the items.

- [K-Dense-AI Scientific Agent Skills](https://github.com/K-Dense-AI/scientific-agent-skills)
A comprehensive collection of over 160 ready-to-use scientific and research skills... very strongly geared toward biology and life sciences, but unquestionably some of the tools could be used elsewhere. Portable agent plugins package. [Thanks to Allen Lee for mentioning]

- [mcptools](https://posit-dev.github.io/mcptools/) and [btw](https://posit-dev.github.io/btw/) — Posit (R session integration). Very focused on bridging R and its quirky toolset, like connecting to the R session from an agent.

- [BioMCP](https://biomcp.org/) — GenomOncology (biomedical data access). BioMCP is a biomedical command-line interface and MCP server designed for practical research and clinical-informatics workflows. Interesting in that frontier models might just generate these tools on the fly (certainly GPT 5.5 could access GEO): that *would* seem to be a waste of tokens, though. Available as a command-line tool and MCP server; most queries work without credentials, but some sources [require API keys](https://biomcp.org/getting-started/api-keys/).

### Supporting tools and integration (Non-AI)

- [Observable](https://observablehq.com/) This is the "commercial"(?) arm to what will be the far more familiar D3, but very noticeably this project has changed in the last few months to be "agent first." Maybe this will be a trend. From the new release announcement: "Rather than obviating the need to understand code, we believe our mission to make code more accessible is more urgent than ever. We reimagined how computational notebooks could work with agents as the primary interface. Our new agent-first notebooks, called chats, are radically different from our human-first notebooks and yet seamlessly interoperate with them."

- [Marimo](https://marimo.io/) A Jupyter notebook alternative presented in the same vein as Observable. Now includes direct LLM integration.

### Other

- SciML is a [very impressive](https://github.com/SciML) public scientific resource built in Julia. Coding agents are a major part of the contributing team, and so are humans. Note the lack of agent-facing documents or dotfiles (though, contributing is also a bit guarded).

### Older items

This section reserved for items that "graduate" off the list due to age (likely in months).

## Submitting New Resources

Did we miss something? Is there a great new resource out there you find particularly useful? Please let us know: the best way to do this is submit your own PR.
