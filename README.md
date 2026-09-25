AI Disclosure: Some of my github projects are presented with AI-assisted writing that I've reviewed. You'll see an indicator on the project README is that's the case. If you would like to check out my fully-human thoughts on my projects, please see my personal website [cassie.mccoy.world](https://cassie.mccoy.world)!

# Cassandra McCoy

Hey! I work on research, threat modeling, human-authored behavioral testing, and applied evals across three main areas: decentralized alignment and character evaluations, agentic cyber risks, and the under-explored field of emergent Neuralese and steganography in multi-agent-human interactions.

## Selected projects

### [MoE Circuit Discovery](https://github.com/c4554ndr4/moe-circuit-discovery) · Neural circuit discovery

MoE circuit discovery is a toolkit to identify a small set of neurons involved in a behavior from 10–50 examples. On my original adult overrefusal sample, measured refusals dropped from 72% to 0% on a held-out test set. A later replication with reconstructed neuron masks found no clear aggregate regression from baseline on a 570-question MMLU subset; a lower refusal rate does not necessarily mean a completed answer.

I tried a few methods of selecting neurons only from experts whose routing looked refusal related, using learned expert selection, but found that simply selecting the strongest contrast-ranked neurons worked best among the methods I tested.

[Read the project](https://github.com/c4554ndr4/moe-circuit-discovery#readme)

### [Scout Browser](https://github.com/c4554ndr4/nextgen_browser_app) · Decentralized alignment

Scout Browser was a research project to build an alignment monitor designed to simultaneously serve multiple principals: parents and their children. The project required a sophisticated model of risk to children via YouTube and the web at large. To create an intermediary model that filters content, the model had to learn (via ICL) which types of content were misaligned with the parent’s preferences, or in the absence of parental preference, general child safety.

The project involved building one of the first instances of continual preference adaptation for live and iterative child-safety filtering, based on a web agent with the often competing alignment interests of both parents and children. Solving for this constraint involved teaching the model how to operate across multiple decision boundaries within a single turn before deciding on the content to serve the user.

[Read the project](https://github.com/c4554ndr4/nextgen_browser_app#readme) · [Research essay](https://cassie.mccoy.world/publish/Research/Alignment%20Write-Ups/Decentralized%20Alignment%20in%20Web%20Agents%20Serving%20Parent-Child%20User%20Pairs)

### [Emergent Edge](https://github.com/c4554ndr4/emergent-edge) · Edge-case user detection pipeline

Emergent edge is a pipeline that sources new edge-case user behavior from reddit and personal blogs. It's important for frontier labs to understand how their models are being used because sometimes model spec violations are not easy to detect using aggregate statistics over production data or other internal methods. For example, the GPT4o spiralism phenomenon proliferated on reddit before OpenAI caught wind and addressed it. This project sources posts that also bring up interesting questions about how the model should behave in certain situations. Example patterns I detected include users being distressed about AI dependency on the My Boyfriend is AI subreddit and individuals writing blog posts about tool injection attacks that they surfaced. 

[Explore the cases](https://emergent-edge-case-ai-use-detector.vercel.app) · [Read the project](https://github.com/c4554ndr4/emergent-edge#readme)

### [The Bad Timeline](https://github.com/c4554ndr4/the-bad-timeline) · Cognitive (In)security Demo

A Twitter replica we built for DEF CON, originally using Kimi-K2 on Groq. Likes and stated preferences shape the next batch of posts, alongside an operator-defined objective. One generation process appears as many authors: a personalized feed can make an operator's position feel like independent social agreement. The README explains that mechanism, the responsiveness goal, and the differences between the original demonstration and later implementation.

[Read the project](https://github.com/c4554ndr4/the-bad-timeline#readme)

### [SymWrite](https://github.com/c4554ndr4/sym-write) · Memory and authorship

Which parts of someone's earlier writing should influence their next thought? SymWrite retrieves a small set of excerpts, explores five continuations in parallel, and offers an optional refinement beside those alternatives. The writer can inspect the selected context and decide what enters the draft.

[Read the project and examples](https://github.com/c4554ndr4/sym-write#readme)

### [Living Dreaming Symbionts](https://github.com/c4554ndr4/living-dreaming-symbionts) · Verifiable outcomes

A research toolkit for checking structured evidence against an agreed goal and producing an independently verifiable receipt. A valid proof can say that the goal was not met. The architecture separates correctness of the calculation from the harder questions of whether the evidence is true, complete, or attributable to an agent.

[Read the project](https://github.com/c4554ndr4/living-dreaming-symbionts#readme)

### [Discord Symbiont](https://github.com/c4554ndr4/Discord_Symbiont) · Persistent assistants

My 2025 Discord application combines conversation context, semantic memory, model routing, tool dispatch, and budget tracking. It is a useful sample of the surrounding architecture needed to make model interactions persist across conversations.

### [Personal Site Dungeon Crawler](https://github.com/c4554ndr4/portfolio) · Playable navigation

A small dungeon serves as the entrance to my writing and projects. Proximity reveals a portal's destination; entering it opens an ordinary website page. A direct Link View reaches the same content. The interesting connection is between movement through a room and navigation through ideas.

[Play the dungeon crawler](https://c4554ndr4.github.io/portfolio/) · [Read the project](https://github.com/c4554ndr4/portfolio#readme)

### [Lens-flare ray tracing](https://github.com/c4554ndr4/lens_flare_demo/blob/9579e7fc5e181089e3c993537360516fda6f668c/camera_model.ipynb) · Graphics algorithms

I implemented ray and ghost tracing in Python/NumPy for a Spring 2021 graphics project based on [Physically-Based Real-Time Lens Flare Rendering](https://resources.mpi-inf.mpg.de/lensflareRendering/) (Hullin et al., SIGGRAPH 2011). My notebook explores optical transfer matrices, two-reflection ghost paths, wavelength-dependent refraction, and aperture handling. The link points directly to my IPython notebook implementation.

These samples include individual projects, team contributions, and work built on existing applications. The READMEs identify those boundaries, distinguish original research from later restoration, and describe what I would improve next. Several public repositories begin with reviewed snapshots; their first public commit dates are not the dates the projects began.
