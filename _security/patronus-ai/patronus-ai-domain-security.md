---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: patronus.ai
  spf: true
hosts:
- cert_expires: Aug 17 12:15:50 2026 GMT
  host: www.patronus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: docs.patronus.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patronus Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patronus AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Patronus AI
provider_slug: patronus-ai
slug: patronus-ai-domain-security
source_filename: patronus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patronus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.patronus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: patronus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patronus-ai/refs/heads/main/security/patronus-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- LLM Evaluation
- Guardrails
- Judges
- Hallucination Detection
- AI Research
- Benchmarks
- API
---
