# Awesome AI Security

[![HOL Guard](https://img.shields.io/badge/HOL%20Guard-secure%20AI%20agents-00a67e)](https://hol.org/guard)
[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

A curated list of open-source tools, frameworks, and resources for securing AI agents and coding assistants.

## Contents

- [Static Analysis & Scanners](#static-analysis--scanners)
- [Runtime Protection](#runtime-protection)
- [MCP & Plugin Security](#mcp--plugin-security)
- [Supply Chain](#supply-chain)
- [Prompt Injection Defense](#prompt-injection-defense)
- [Resources](#resources)

## Static Analysis & Scanners

Tools that scan AI agent plugins, skills, and configurations for vulnerabilities before deployment.

- **[HOL Guard](https://github.com/hashgraph-online/hol-guard)** — Open-source security scanner for AI coding agents. 130-point scoring across 7 categories. Supports Claude Code, Codex, Cursor, Gemini. [PyPI](https://pypi.org/project/plugin-scanner/)
- **[OpenSSF Scorecard](https://github.com/ossf/scorecard)** — Security health checks for open source projects. Not AI-specific but critical for any dependency.
- **[Bandit](https://github.com/PyCQA/bandit)** — Python security linter. Catches common issues in AI agent Python code.
- **[Semgrep](https://github.com/semgrep/semgrep)** — Lightweight static analysis. Good for custom security rules on agent code.

## Runtime Protection

Tools that intercept and protect AI agents during execution.

- **[HOL Guard Agent Shield](https://hol.org/guard)** — Runtime protection with 4 levels: Gentle, Balanced, Strict, Paranoid. Intercepts malicious operations in real-time.
- **[Cisco AI Defense](https://www.cisco.com/site/us/en/products/security/ai-defense.html)** — Enterprise AI security platform. Integrates with HOL Guard for deep scanning.
- **[Guardrails AI](https://github.com/guardrails-ai/guardrails)** — Input/output validation for LLM applications. Not agent-specific but useful.

## MCP & Plugin Security

Security around Model Context Protocol servers and plugins.

- **[HOL Plugin Scanner](https://pypi.org/project/plugin-scanner/)** — CLI tool for scoring MCP plugins and Codex skills. 7-category analysis including manifest validation, secrets detection, and code quality.
- **[HOL Guard CI Action](https://github.com/hashgraph-online/ai-plugin-scanner-action)** — GitHub Action that runs the scanner on every PR. Fails on score < 80 or high/critical findings.
- **[Awesome Codex Plugins](https://github.com/hashgraph-online/awesome-codex-plugins)** — Curated list of Codex plugins. **HOL Guard scanning is now mandatory for inclusion.**
- **[MCP Inspector](https://github.com/modelcontextprotocol/inspector)** — Official tool for testing MCP servers. Useful for understanding what an MCP server can do before installing it.

## Supply Chain

- **[SLSA](https://github.com/slsa-framework/slsa)** — Supply-chain Levels for Software Artifacts. Framework for provenance and integrity.
- **[Sigstore](https://github.com/sigstore)** — Signing, verification, and provenance for open source software.
- **[Dependabot](https://github.com/dependabot)** — GitHub-native dependency updates. Enable it on every AI agent plugin repo.

## Prompt Injection Defense

- **[Rebuff](https://github.com/protectai/rebuff)** — Prompt injection detection. Open-source but maintenance status unclear.
- **[LLM Guard](https://github.com/laiyer-ai/llm-guard)** — Input/output scanners for LLM applications. Anonymization, toxicity, and injection detection.
- **[Purple Llama](https://github.com/meta-llama/PurpleLlama)** — Meta's suite for AI safety including prompt injection benchmarks.

## Resources

- **[HOL Guard Docs](https://hol.org/guard)** — Official documentation and protection level reference.
- **[Cisco AI Defense Blog](https://blogs.cisco.com/tag/ai-defense)** — Enterprise AI security research and threat intelligence.
- **[OWASP LLM Top 10](https://owasp.org/www-project-top-10-for-large-language-model-applications/)** — Standardized risks for LLM applications.
- **[AI Village](https://aivillage.org/)** — Community for AI security research and red-teaming.

## Contributing

Know a tool that should be here? Open a PR. All listed tools must be open source and actively maintained.

## License

This list is [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
