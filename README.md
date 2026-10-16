# Awesome-Linters-Code-Quality

## Top Linters & Code Quality Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Static Analysis, Security Scanning & Code Quality Automation*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Linters & Code Quality**. These tools perform static analysis, security scanning, code smell detection, and quality metric tracking to catch bugs and vulnerabilities before code reaches production.



**Examples** include SonarQube, Veracode, Checkmarx, Codacy, Code Climate, DeepSource, Coverity, Snyk Code, GitHub Advanced Security, and Qodana (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, language-specific analysis, and transparent security scanning — ideal for developers, platform teams, and organizations building vendor-neutral code quality pipelines.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[SonarQube](https://www.sonarsource.com/)**  

  Leading code quality platform with Community Edition free (LGPL v3). Covers 30+ languages with code smell detection, complexity metrics, and technical debt tracking. Security rules for taint analysis require paid Developer/Enterprise editions .



- **[Veracode](https://www.veracode.com/)**  

  Enterprise application security platform with SAST, DAST, SCA, and manual penetration testing services.



- **[Checkmarx](https://checkmarx.com/)**  

  Enterprise SAST/SCA platform with codebases scanning, software composition analysis, and developer-friendly integrations.



- **[Codacy](https://www.codacy.com/)**  

  Automated code review platform with quality, security, duplication, and coverage tracking; SaaS with self-hosted option.



- **[Code Climate](https://codeclimate.com/)**  

  Engineering intelligence platform with maintainability checks, test coverage tracking, and velocity metrics.



- **[DeepSource](https://deepsource.com/)**  

  AI-powered code review with static analysis, security scanning, and automated fixes for 10+ languages.



- **[Coverity](https://www.synopsys.com/)**  

  Synopsys enterprise static analysis platform known for deep defect detection across C/C++, Java, C#, and more.



- **[Snyk Code](https://snyk.io/)**  

  AI-powered SAST integrated into Snyk's security platform; free tier for open source projects.



- **[GitHub Advanced Security](https://github.com/features/security)**  

  CodeQL-powered code scanning bundled with GitHub Enterprise; free for public repositories .



- **[Qodana](https://www.jetbrains.com/qodana/)**  

  JetBrains' code quality platform with deep IDE-integrated analysis for Java, Kotlin, Python, and JavaScript.



## Open-Source GitHub Projects



- **[ESLint](https://github.com/eslint/eslint)**  

  **The standard linting tool for JavaScript and TypeScript** — 27,000+ stars, the most widely adopted linter with 134 million weekly npm downloads. Huge plugin ecosystem covering code quality, style, accessibility, and security checks. Supports auto-fix for most rules .



- **[Semgrep](https://github.com/semgrep/semgrep)**  

  **The most widely adopted open-source SAST tool** — pattern-based scanning that looks like the code it matches. Supports 30+ languages with a large public rule registry. Fast enough for pre-commit hooks. LGPL-2.1 licensed .



- **[CodeQL](https://github.com/github/codeql)**  

  **GitHub's semantic code analysis engine** — treats source code as a queryable database with powerful data-flow queries. Free for public repositories. Default rule packs for C/C++, Java, JavaScript, Python, Go, and C# are well-maintained. Steeper learning curve than Semgrep .



- **[Biome](https://github.com/biomejs/biome)**  

  **Rust-based linter and formatter** — 24,000+ stars, ~20x faster than ESLint on large codebases. Single tool for linting, formatting, and import organization. v2.x added type-aware rules without running the full TypeScript compiler .



- **[Oxlint](https://github.com/oxc-project/oxc)**  

  **Fastest JavaScript/TypeScript linter** — processes ~11,774 files/second (2.5x faster than Biome). 865+ built-in rules ported from ESLint, typescript-eslint, react, jest, and more. Backed by Cloudflare through VoidZero. Type-aware mode via tsgolint .



- **[Ruff](https://github.com/astral-sh/ruff)**  

  **High-performance Python linter written in Rust** — 10-100x faster than Flake8/Pylint. Replaces multiple tools (flake8, isort, pyupgrade, autoflake) in a single binary. Supports auto-fix and is quickly becoming the Python linting standard .



- **[Pylint](https://github.com/pylint-dev/pylint)**  

  **Most configurable Python linter** — checks style, type consistency, and common errors. Per-module scoring tracks quality over time. Plugin-based architecture for custom checks. W0611 (unused imports), W0102 (dangerous default values), and C0302 (module too long) are especially valuable for AI-assisted codebases .



- **[Bandit](https://github.com/PyCQA/bandit)**  

  **Security-focused static analysis for Python** — 6,000+ stars, MIT licensed. Finds common security issues (eval, pickle, hardcoded passwords, SQL injection patterns). Low false-positive rate, CI integration. Created because Python lacked a security-focused linter .



- **[gosec](https://github.com/securego/gosec)**  

  **Security-focused static analysis for Go** — 7,500+ stars, Apache-2.0. Scans Go AST for security issues with CWE identification and SARIF output. Pairs well with golangci-lint .



- **[Brakeman](https://github.com/presidentbeef/brakeman)**  

  **Security scanner for Ruby on Rails** — MIT licensed. Over 90 distinct check types for Rails-specific patterns including mass assignment, unsafe render calls, and SQL injection. Built because generic linters missed Rails idioms .



- **[SpotBugs](https://github.com/spotbugs/spotbugs)**  

  **Static analysis for Java** — successor to FindBugs with active development and modern Java support. FindSecBugs plugin adds ~140 security-specific bug patterns. LGPL-2.1 licensed .



- **[PMD](https://github.com/pmd/pmd)**  

  **Source code analyzer for Java, JavaScript, Apex, and more** — finds programming flaws, dead code, suboptimal code, and overcomplicated expressions. Includes copy-paste detection (CPD). Maven/Gradle/IDE integration .



- **[Trivy](https://github.com/aquasecurity/trivy)**  

  **Comprehensive security scanner** — 21,000+ stars, Apache-2.0. Covers vulnerabilities, misconfigurations, secrets, containers, filesystems, and IaC. Fast single-binary deployment. No SAST but fills the SCA/container scanning gap .



### Additional Strong Open-Source Options



- **[Opengrep](https://github.com/opengrep/opengrep)** — Fork of Semgrep v1.100 created after Semgrep's Dec 2024 relicense. LGPL-2.1, backed by ~10 vendors. Rule ecosystem tracks Semgrep CE. Use as licensing hedge .

- **[ast-grep](https://github.com/ast-grep/ast-grep)** — Rust-native structural search tool, MIT licensed. Fast with SARIF output. Pairs well with Semgrep for interactive variant analysis .

- **[golangci-lint](https://github.com/golangci/golangci-lint)** — Meta-linter for Go running multiple linters in parallel. Configure gosec, gocritic, unparam, and staticcheck explicitly .

- **[Cppcheck](https://github.com/danmar/cppcheck)** — Static analysis for C/C++ detecting bugs compilers miss. Portable, no syntax error detection .

- **[Flawfinder](https://github.com/david-a-wheeler/flawfinder)** — One of the oldest C/C++ security tools (2001). GPL-2.0. Reports possible weaknesses sorted by risk .

- **[phpmetrics](https://github.com/phpmetrics/PhpMetrics)** — PHP code metrics with readable HTML reports .

- **[ShellCheck](https://github.com/koalaman/shellcheck)** — Finds bugs in shell scripts .



**Frameworks for building custom systems**: Combine **ESLint** or **Biome** for JS/TS linting, **Semgrep** for cross-language security scanning, **CodeQL** for deep data-flow analysis, and language-specific tools (**Bandit**, **gosec**, **Brakeman**) for framework-specific footguns. Layer in **Trivy** for container/dependency scanning. For Python, **Ruff** + **Pylint** + **Bandit** provides comprehensive coverage .



**Key architectural insight**: Open-source SAST tools catch real bugs but miss supply-chain flaws like Log4Shell entirely — pair with SCA tools. Language-specific linters have lower false-positive rates than general-purpose scanners for their target issue classes. The union of ESLint + Semgrep + CodeQL findings is usually more valuable than any single tool alone .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- **License awareness is critical**: SonarQube Community Edition is LGPL v3; security rules require paid tiers. Semgrep core is LGPL-2.1 with proprietary Pro tier. Opengrep is a licensing hedge for teams uncomfortable with Semgrep's commercial gating .

- Open-source SAST tools don't ship compliance mappings (SOC 2, PCI-DSS), centralized dashboards across hundreds of repos, or vendor support contracts. They provide raw findings — you own triage .

- Self-hosted solutions require CI/CD integration, rule tuning, and ongoing maintenance.



---



**Made for developers, security engineers, platform teams, and code quality advocates.**  

Let's make code quality more open, automated, and vendor-neutral.
