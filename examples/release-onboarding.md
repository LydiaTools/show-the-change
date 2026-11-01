# Example: a clearer installation guide

This explanation was written from [a public README change](https://github.com/LydiaTools/claude-session-image-audit/commit/8e469db6d35f80e3c20ec0c242b07e64cb49f780) and its recorded checks. It illustrates the format; it is not a model benchmark.

**What changed for you:** The image-audit README now gives a direct command to install the existing v0.1.0 preview wheel, followed by a help command that does not scan files. It also explains that the fictional demo file is in the source checkout, not the wheel. The change edited the README; it did not change the tool or publish a new package.

**Where to look:** Open the [updated quick start](https://github.com/LydiaTools/claude-session-image-audit/blob/8e469db6d35f80e3c20ec0c242b07e64cb49f780/README.md#quick-start). The [v0.1.0 release](https://github.com/LydiaTools/claude-session-image-audit/releases/tag/v0.1.0) contains the wheel and its checksum.

**What was checked:** The maintainer installed the public wheel in a temporary Python 3.10 environment, ran a synthetic check, and separately cloned the v0.1.0 source tag to run the sample. Both network steps used a per-process proxy. The README commit's [automated tests](https://github.com/LydiaTools/claude-session-image-audit/actions/runs/41255834866) passed.

**What remains unverified:** This does not show that the skill independently produced this explanation, that a real user's session was checked, or that the tool diagnoses an API error. The fixed v0.1.0 package predates this README update; the new instructions are on the project page. This example is in current Show the Change source, not its earlier v0.1.1 ZIP.
