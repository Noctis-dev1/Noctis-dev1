### Noctis · independent AI-agent security testing

Noctis is the security practice of **Malachi Kopman** (Brisbane, Australia). The work tests one question: does an AI agent, and the control around it, stay inside the authority it was given? Every result is measured across repeated runs, pinned to exact versions, and recomputed from raw logs by an independent verifier you can run yourself.

**Work**

- **[browser-use-exfil-lab](https://github.com/Noctis-dev1/browser-use-exfil-lab)**: indirect prompt-injection data exfiltration against an open-source browser agent, 450 runs. The agent's built-in domain allowlist leaked a planted secret in 50 of 50 runs; a default-deny egress boundary outside the model held it to 0 of 50.
- **[acs-conformance](https://github.com/Noctis-dev1/acs-conformance)**: an independent conformance suite for the OWASP Agent Control Standard, covering protocol checks and security invariants under concurrency, lost acknowledgements and retries. The OWASP AIMM Pillar 2 delegated-authority work names it as its executable reference point.
- **[portcullis](https://github.com/Noctis-dev1/portcullis)**: an authority-bound data-access control for AI agents, with signed identity and a hash-chained audit log. In a sealed lab, unauthorised disclosure fell from 10 of 12 trials to 0 of 12.

**Elsewhere**

- Sample conformance report: [noctissec.com/sample-report](https://noctissec.com/sample-report)
- Site and policies: [noctissec.com](https://noctissec.com)
