# Amfelt

Amfelt automates the groundwork of a data platform. An agent runs on your infrastructure, inspects your source systems and describes them in contracts based on the [Open Data Contract Standard](https://bitol-io.github.io/open-data-contract-standard/). From those contracts Amfelt generates the data layers and load logic, and your team decides how each dataset keeps its history.

We're preparing Amfelt for its first teams. You can [try the live demo](https://amfelt.com/go/demo/?utm_source=github&utm_medium=social&utm_campaign=org-profile) or [join the waitlist](https://amfelt.com/waitlist/?utm_source=github&utm_medium=social&utm_campaign=org-profile).

## What's public here

The platform itself is developed in private repositories, so this page stays small for now. These are the repositories you can use or read today:

| Repository | What it is |
| --- | --- |
| [demo-static-gating](https://github.com/amfeltlabs/demo-static-gating) | A Hugo site embedded in a Go binary, served only to readers with a Hanko session and a role you granted. A runnable proof of concept, not a hardened server. |
| [homebrew-tap](https://github.com/amfeltlabs/homebrew-tap) | Homebrew formulae for the `amfelt` agent. Nothing is published yet, so it can't install the agent today. |
| [scoop-bucket](https://github.com/amfeltlabs/scoop-bucket) | Scoop manifests for the `amfelt` agent. Nothing is published yet, so it can't install the agent today. |

## How we build it

The control plane is a Go modular monolith with a Hugo and HTMX front end, and connectors exchange data as [Apache Arrow](https://arrow.apache.org) record batches. We write about those decisions on our blog:

- [We skipped microservices and built a modular monolith](https://amfelt.com/blog/why-our-platform-is-a-modular-monolith/?utm_source=github&utm_medium=social&utm_campaign=org-profile)
- [We chose HTMX over React for our app](https://amfelt.com/blog/htmx-instead-of-react/?utm_source=github&utm_medium=social&utm_campaign=org-profile)
- [Keep the site static, put a Go server in front of it](https://amfelt.com/blog/gating-a-static-site-with-go/?utm_source=github&utm_medium=social&utm_campaign=org-profile)
- [How we keep parallel agents working toward the same plan](https://amfelt.com/blog/coordinating-parallel-agents/?utm_source=github&utm_medium=social&utm_campaign=org-profile)

Questions or ideas? Reach us at [hello@amfelt.com](mailto:hello@amfelt.com).
