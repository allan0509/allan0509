# Hi, I'm Allan

I work on AI platforms, agent evaluation, and the runtime systems that make agents more reliable in real-world use.

My current interests include:

- Agent evaluation workflows, from requirements and case design to runs, diagnostics, and reports
- Agent runtimes, session lifecycle, MCP tooling, and long-running task reliability
- Tool and skill ecosystems that connect models with real product and business workflows

## Selected open-source contributions

### OpenClaw

- **[Session-scoped MCP runtime cache](https://github.com/openclaw/openclaw/pull/55090)** — merged into `main`. Reused bundled MCP runtimes and tool catalogs across turns, invalidated them when configuration changed, and disposed stale runtimes on session rollover.
- **[Feishu streaming-card delivery](https://github.com/openclaw/openclaw/pull/53534)** — improved throttling, pending flushes, and duplicate-card handling. The maintainers rebased the work into the [canonical merged implementation](https://github.com/openclaw/openclaw/pull/71523) and preserved contributor credit in the changelog.
- **[Codex ACP no-output stall diagnosis](https://github.com/openclaw/openclaw/issues/44810)** — reproduced an environment-dependent child-session stall, separated it from authentication and runtime-mode issues, and proposed lifecycle diagnostics. The resulting fix now distinguishes pre-prompt stalls, no-runtime-event stalls, runtime-active/no-visible-output stalls, and true interactive waits.

Other areas I have explored in OpenClaw include heartbeat session isolation, Feishu connection health, runtime recovery, and service-specific permission tooling.

## How I work

I prefer to start from a real failure or user workflow, establish a reproducible evidence chain, and then narrow the solution into a reviewable change with explicit lifecycle boundaries and regression coverage.

