---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: confident-ai.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: deepeval.com
  spf: false
hosts:
- cert_expires: Sep 24 05:05:58 2026 GMT
  host: www.confident-ai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 15:00:18 2026 GMT
  host: deepeval.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepeval Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepEval, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: DeepEval
provider_slug: deepeval
slug: deepeval-domain-security
source_filename: deepeval-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.confident-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 05:05:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: deepeval.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:00:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: confident-ai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: deepeval.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepeval/refs/heads/main/security/deepeval-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- LLM Evaluation
- LLM Testing
- Evaluation Framework
- Evaluation Metrics
- LLM Observability
- LLM as a Judge
- G-Eval
- RAG Evaluation
- Agent Evaluation
- Hallucination Detection
- Bias Detection
- Toxicity Detection
- Red Teaming
- Benchmarks
- MMLU
- Synthetic Data Generation
- Prompt Optimization
- CI CD
- Pytest
- Python
- Open Source
- Apache 2.0
- MCP
---
