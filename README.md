### Oscar Guirado

I build infrastructure for AI agents: isolated places for them to act, deterministic routers over large codebases, and evidence you can check instead of trust.
Linux, low level, Rust, Go and Python. Every project below states its own limits next to its results.

#### Projects

**[ViewPoint](https://github.com/oguirado/ViewPoint)** · Rust · Go · Python · Electron + Vue · AGPL-3.0
A Linux desktop where a person and AI agents work the same real programs, each in its own capsule, on one wall. In this hackathon build the agents are Gemini.
Every agent action is checked against a fresh screen frame before it counts, capsules can be rewound, and a human can take control back at any time. Built on the MetaViewer core.
CI and the quickstart run on x86_64 and ARM64.
[Live demo](https://viewpoint-swarm-viewer-dtrnknr6bq-ew.a.run.app) · [2-min video](https://www.youtube.com/watch?v=k-59hnctF6M)

**[TaskLight](https://github.com/oguirado/TaskLight)** · TypeScript · Python · Firebase AI Logic · AGPL-3.0
A shared control plane and live task wall for developers who run several AI agents at once. Agents append plans, tasks and memory to a local room log over MCP (34 tools, 6 planning templates); a native host relays them through a Chrome extension to a wall that shows who is doing what and what is blocked.
Swarm narration runs on-device with Gemini Nano; private rooms never leave the device, and the narrator cannot change the plan.
Firebase hosting is not deployed yet; a local demo runs the full path without it.
*Firebase #BuildHybridAI hackathon.*

**[Lineage](https://github.com/oguirado/Lineage)** · Python (standard library only) · TypeScript UI · AGPL-3.0
A local laboratory for developers who run coding agents: give agents an identity and evidence-backed memory, measure them on runs and benchmarks, breed variants (clone, distill, cross, mutation), and promote or retire them only on evidence.
Every change is an event in an append-only, hash-chained ledger that can be verified independently. One registry of 38 tools serves the CLI, MCP, a file mailbox and a web UI.
Early preview: the backend is tested; the guided quickstart and end-to-end demo are still being written.

**[LinuxDistill](https://github.com/oguirado/LinuxDistill)** · Python · GPL-2.0
A pinned, verified map of the Linux kernel for AI agents: a deterministic router over 8,182 files and 138,451 symbols (no model, about 0.4 s per query), plus 111,144 model-written findings, each linked to the code it cites.
It ships no kernel source: a script fetches the exact upstream snapshot and checks every file's hash. Findings are leads, not facts: in a review of 136 of them, 47% were fully supported.

**[math-router](https://github.com/oguirado/math-router)** · Python · Apache-2.0
A routable edition of the 719 math preprints in OpenAI's math repository, with an offline router that answers in at most 2,000 bytes and abstains when support is weak.
Graded benchmark: hit@5 0.85 on 39 answerable test queries (R@1 0.22). 14 gates and both benchmark runs reproduce in CI. Unofficial, not affiliated with OpenAI.

<!--
#### Selected Upstream Contributions
Uncomment this section once the first pull request is merged. Merged PRs only, one line each:
- **[project#NNNN](https://github.com/org/project/pull/NNNN)**: what it fixed, and the measured impact (memory, latency, a fixed race condition)
-->
