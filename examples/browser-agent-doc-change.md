# Example: a documentation change

The following explanation was written by inspecting [commit `82d801b`](https://github.com/LydiaTools/browser-agent-blueprint/commit/82d801b9228f815fccda9b50f5dfd98290fabacb) and its recorded checks. It is an example of the desired format, not a model benchmark.

**What changed:** The browser-agent guide now explains that a pinned tab and a successful click response do not prove a save completed. It links a reported upstream issue and suggests checking the actual record afterward. This commit changed two documentation files; it did not change the browser tool.

**Where to look:** Open the [English guide](https://github.com/LydiaTools/browser-agent-blueprint/blob/82d801b9228f815fccda9b50f5dfd98290fabacb/docs/agent-browser-pinned-sessions.md#a-pinned-tab-is-not-an-action-receipt). Read “A pinned tab is not an action receipt.”

**What was checked:** The contribution's two GitHub Actions runs passed, and the source commit was merged. The maintainer also recorded a local synthetic test; its tabs reported visible, so it did not reproduce the upstream hidden-tab scenario.

**What this does not show:** The fixed v0.2.5 ZIP predates this documentation. This commit does not prove that any browser issue was fixed or that a real website was tested.
