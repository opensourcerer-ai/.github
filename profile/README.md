# OpenSourcerer AI

OpenSourcerer AI builds open-source tools for **AI-assisted security, cryptography, and repository analysis**.

The organization focuses on practical engineering tools that help teams inspect codebases, verify security-related assumptions, and improve reliability in systems that must remain maintainable over time.

Rather than treating AI as a substitute for engineering discipline, these projects use AI where it is useful while keeping the work grounded in reviewable outputs, explicit controls, and real software concerns.

---

## Core Principles

### Engineering First

AI is a tool, not a replacement for sound engineering.

Projects in this organization are built to support real software work: analysis, verification, security review, and cryptographic integration.

---

### Explicit Control

Reliable systems depend on clear constraints, reviewable outputs, and mechanisms that make problems visible.

The goal is not opaque automation, but tools that help engineers understand what is happening and act on it.

---

### Long-Term Maintainability

Software outlives individual implementations and often outlives the tools used to produce it.

Projects here are developed with an emphasis on maintainability, clarity, and use in long-lived systems.

---

## Projects

### SCA — Security Control Agent

SCA is an AI-assisted repository analysis tool focused on **security controls**.

It evaluates codebases against defined security expectations and control-oriented review criteria, including analysis inspired by:

- **OWASP**
- **NIST**
- cryptographic usage review
- repository security hygiene
- issue-oriented reporting for engineering workflows

Repository:  
https://github.com/opensourcerer-ai/sca

---

### FMA — Failure Mode Agent

FMA is an AI-assisted repository analysis tool focused on **failure modes in software systems**.

It identifies implementation patterns that commonly lead to instability, service failure, unsafe recovery behavior, and operational weakness.

Typical areas of analysis include:

- missing timeouts
- unbounded resource usage
- retry storms
- unsafe concurrency patterns
- missing backpressure or recovery controls
- systemic reliability weaknesses in code and design

Repository:  
https://github.com/opensourcerer-ai/fma

---

### xpkcs11

xpkcs11 is an open cryptographic project centered on **PKCS#11-related tooling and integration**.

It focuses on clarity, portability, and practical support for secure cryptographic workflows in environments that rely on standard key management interfaces.

Repository:  
https://github.com/opensourcerer-ai/xpkcs11

---

## Writing

Roger Allan writes about AI systems, software reliability, cryptography, and engineering practices for AI-assisted development.

Substack:  
https://rogerallan.substack.com

---

## License

Each repository contains its own license information.
