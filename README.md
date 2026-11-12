### Oscar Guirado

I build infrastructure for AI agents: isolated places for them to act, deterministic routers over large codebases, and evidence you can check instead of trust.
Linux, low level, Rust, Go and Python. Every project below states its own limits next to its results.

#### Projects

**[MetaViewer](https://github.com/oguirado/MetaViewer)** · Rust · Go · Electron · AGPL-3.0
A Linux desktop wall where a person and an AI agent share programs and browsers in capsules: containers, and on ARM64 VMs and MicroVMs with rewind.
Every agent action must name its target and the frame it saw; a Rust core checks both before dispatch and records decisions in a journal that `mv-replay` can verify.
*Meta Global AI Developer Hackathon.*

**[LinuxDistill](https://github.com/oguirado/LinuxDistill)** · Python · GPL-2.0
A pinned, verified map of the Linux kernel for AI agents: a deterministic router over 8,182 files and 138,451 symbols (no model, about 0.4 s per query), plus 111,144 model-written findings, each linked to the code it cites.
It ships no kernel source: a script fetches the exact upstream snapshot and checks every file's hash. Findings are leads, not facts: in a review of 136 of them, 47% were fully supported.

**[math-router](https://github.com/oguirado/math-router)** · Python · Apache-2.0
A routable edition of the 719 math preprints in OpenAI's math repository, with an offline router that answers in at most 2,000 bytes and abstains when support is weak.
Graded benchmark: hit@5 0.85 on 39 answerable test queries (R@1 0.22). 14 gates and both benchmark runs reproduce in CI. Unofficial, not affiliated with OpenAI.

**[Café](https://github.com/oguirado/cafe)** · Rust · Python · Electron + Vue
A Windows app for Twitch streamers: one clean recording per Discord window (Windows Graphics Capture + FFmpeg/NVENC), one-click OBS scenes, and Twitch chat that Codex can read over MCP.
Tested on one laptop only; the README lists what is still unverified.
*Codex x TwitchCon Hackathon.*

<!--
#### Selected Upstream Contributions
Uncomment this section once the first pull request is merged. Merged PRs only, one line each:
- **[project#NNNN](https://github.com/org/project/pull/NNNN)**: what it fixed, and the measured impact (memory, latency, a fixed race condition)
-->
