# Hi, I’m Ioan 👋

I’m a Lead Engineer at ImmoScout24 Austria, building search platforms and APIs. I’ve been with the company for 10+ years.

I’m a dad of four (yes, four), into music and guitar, and a Home Assistant enthusiast. After eight years in Austria, I’m now based in Sibiu, Romania.

I started in control theory and automation engineering, then found my place in software. AI workflows have brought back my love of automation. Apparently, I’ve come full circle. Or closed the loop.

At work I still build things. With my fellow leads and our Head of Technology, I also help decide where our Austrian engineering goes: architecture, engineering standards and what we deliver first.

Right now I’m focused on AI-native engineering: agents that get the context they need, workflows we can reuse, and fast verification. People stay in control.

## Things I’ve built and helped shape

- **[Property-search platform](https://www.is24.at/regional/wien/wien/wohnungen)** — I led the architecture of the 2018–2019 relaunch and built core parts of it: streaming React SSR, the first GraphQL search API and the Elasticsearch-backed search URLs. Then I led the phased move of the legacy Angular search and Java catalogue onto it. I’ve kept evolving it since, including a rebuilt geographic autocomplete and shape-based regional search. It’s still in production.

- **[Map search](https://www.immobilienscout24.at/regional/wien/wien/immobilien?bottomLeftLat=48.07975844399566&bottomLeftLon=16.174624586138773&topRightLat=48.360432131508&topRightLon=16.584715413861204)** — The map shows a sample of real properties at their actual locations, not cluster centres. I led delivery from feasibility to first production release in three months (2025) and built the Elasticsearch aggregation behind it; its p95 stayed **under 100 ms** in production (team metrics, August–November 2025). Later, customers reported hidden-address listings showing at their true location, so I designed and built stable masking: the pin stays inside the right postal-code area and doesn’t move between visits.

- **AI-assisted fraud review** — Customer Service used to check private listings by hand before publication, weekends included. I led the [Dify](https://dify.ai/)/[Claude on Bedrock](https://aws.amazon.com/bedrock/) integration with them and another engineer: they brought the fraud expertise and the prompt, and manual fallback stays in place. In its June–August 2026 report, Support had **50%** of those checks clearing for immediate publication.

- **AI recommendations** — Live in the Austrian apps since September 2026. I led the Austrian side: data contracts, identity stitching, event pipelines and the app-feed rollout. The German AI Solutions team owned the embedding model, [SageMaker](https://aws.amazon.com/sagemaker/ai/) API and [OpenSearch](https://opensearch.org/) vector search.

- **Natural-language search** — The Austrian team’s query tokenizer turns free-text German property searches into structured search parameters. My part: early spaCy exploration, architecture and design feedback, and helping bring the service into production.

- **Recoverable checkouts** — A failed Salesforce integration step used to mean manual recovery. I rebuilt checkout completion as visible, retryable workflows on [Step Functions](https://aws.amazon.com/step-functions/) and [Lambda](https://aws.amazon.com/lambda/). From July 2025 through September 2026, CloudWatch recorded **50,000+** successful workflow completions across paid and free checkouts, with **4** failures and **2** timeouts.

- **Shared frontend foundations** — I co-created and still maintain the shared React components and build tooling that 23 Austrian applications used in 2026.

- **Agent tooling** — I built versioned rules and reusable review and migration skills for coding agents, plus a tested tool that rewrites legacy Storybook component examples into the current story format. We used it in the Storybook 6→10 upgrade.

## Open source & writing

- **[`makeomatic/redux-connect`](https://github.com/makeomatic/redux-connect/pull/135)** — Contributed React Context support, released in [`v9.0.0`](https://github.com/makeomatic/redux-connect/releases/tag/v9.0.0).

- [Taming asynchronous JavaScript with Promises](https://medium.com/willhaben/taming-asynchronous-javascript-with-promises-c92b58589026) — on the Willhaben engineering blog.

## Side projects, old and new

- **Cortex** — My Home Assistant setup as code, including solar-surplus EV charging and home-energy controls. I use AI agents to audit the setup and develop changes through tests, review and automated deployment.

- **[bes-lyrics](https://github.com/ioanlucut/bes-lyrics)** — Lyrics and chords as code. I built the checks and songbook tooling; others maintain the content.

- **[Remo](https://github.com/ioanlucut/remo)** — Started as my 2014 master’s dissertation: distributed process control through web services.

- **[Revaluate](https://www.producthunt.com/posts/revaluate) · 2015–2017** — Expense tracking: my Java API and most AngularJS logic, a collaborator’s design and most styling.

**Usually somewhere around:** TypeScript, React, Node.js, GraphQL, Elasticsearch and AWS—with Claude Code, Codex and Datadog in the mix.

[CV (PDF)](Ioan%20Lucut%20-%20Search%20and%20Product%20Platforms%20-%20CV.pdf) · [LinkedIn](https://linkedin.com/in/ilucut) · ioan.lucut88@gmail.com
