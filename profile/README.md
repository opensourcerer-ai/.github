# OpenSourcerer AI

Engineering-grade AI tooling for security-critical and long-lived software systems.

The projects here apply invariant-based governance and constraint enforcement to AI-assisted development workflows — defining explicit behavioral boundaries for AI agents operating on codebases, cryptographic systems, and security-sensitive infrastructure.

---

## Methodology

AI agents produce outputs that require constraint. The approach here treats behavioral constraints as first-class engineering artifacts — specified in plain language, version-controlled alongside code, and enforced at the point of AI agent invocation.

Each tool in this organization is built around an invariant set: a formal collection of rules defining what the agent must always do, what it must never do, and when it must stop and report rather than proceed. The invariant set is the unit of governance. The AI agent is the execution engine operating within it.

This methodology draws on classical AI foundations — logic programming, declarative constraint systems, formal specification — applied to the accuracy and reliability problems that arise when generative AI operates on production software.

---

## Projects

### SCA — Security Control Agent

AI-assisted repository security analysis built on 150+ security invariants across six languages. SCA uses Claude Code as a constrained reasoning engine: the invariants define admissible analysis behavior, and the agent applies that reasoning to produce evidence-based audit reports with exact file citations.

Coverage includes language-specific vulnerability patterns (C/C++, Go, Java, JavaScript, Python, Rust), authentication and authorization controls, cryptographic usage, container and Kubernetes hardening, supply chain integrity, privacy compliance (GDPR, CCPA, HIPAA), and AI agent security including MCP tool access and prompt injection vectors.

SCA produces structured output suitable for CI/CD integration, drift tracking between audit runs, and engineering workflow reporting. The agent operates read-only. All output goes to a designated control directory. Analyzed code is never executed or modified.

Repository: [opensourcerer-ai/sca](https://github.com/opensourcerer-ai/sca)

---

### FMA — Failure Mode Agent

AI-assisted repository analysis focused on failure modes in software systems. FMA identifies implementation patterns that commonly produce instability, service failure, unsafe recovery behavior, and operational weakness under production conditions.

Typical analysis targets include missing timeouts, unbounded resource consumption, retry storms, unsafe concurrency patterns, missing backpressure controls, and systemic reliability weaknesses that static pattern-matching tends to miss.

FMA is under active development.

Repository: [opensourcerer-ai/fma](https://github.com/opensourcerer-ai/fma)

---

### xpkcs11

A PKCS#11 3.1 library with extensible token support and post-quantum cryptographic integration. xpkcs11 provides portable, standards-compliant key management interfaces for environments requiring long-term cryptographic durability across algorithm transitions — including ML-KEM and ML-DSA support for post-quantum migration readiness.

Repository: [opensourcerer-ai/xpkcs11](https://github.com/opensourcerer-ai/xpkcs11)

---

## Design Principles

**Explicit control over opaque automation.** Every agent in this organization operates against a published invariant set. The constraints are readable, reviewable, and modifiable by any engineer on the team. Behavior is governed by specification, not by prompt opacity.

**Outputs are advisory.** These tools produce findings and reports for human review. No tool in this organization auto-modifies source code, auto-merges pull requests, or takes automated production action. The human remains in the decision loop.

**Long-term maintainability.** Software systems outlive the tools used to produce them, and frequently outlive the teams that built them. The tooling here is developed with that constraint in mind — readable outputs, stable interfaces, and invariant sets that remain auditable years after initial deployment.

**Engineering-grade AI.** These tools treat AI as a constrained reasoning engine operating within a specified behavioral envelope. The invariant set is the envelope. Accuracy and reliability follow from constraint precision.

---

## Background

The theoretical foundation for this work draws on logic programming, declarative constraint systems, and formal specification methods developed in the classical AI tradition — including Prolog-based constraint satisfaction, relational knowledge representation, and runtime optimization techniques for constrained search.

That foundation applies directly to the governance problems that emerge when AI agents operate on production codebases: defining termination conditions, constraining search over solution spaces, specifying what must hold across all executions, and identifying when an agent must stop rather than proceed.

---

## Writing

Roger Allan writes about AI systems, software reliability, cryptography, and constraint-based engineering practices.

Substack: [rogerallan.substack.com](https://rogerallan.substack.com)

---

## License

Each repository contains its own license information. SCA and FMA are released under Apache License 2.0. xpkcs11 is released under MIT.
