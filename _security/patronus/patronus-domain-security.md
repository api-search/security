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
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.patronus.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Patronus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Patronus AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Patronus AI
provider_slug: patronus
slug: patronus-domain-security
source_filename: patronus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.patronus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 12:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.patronus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.patronus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: patronus.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/patronus/refs/heads/main/security/patronus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Evaluation
- GenAI
- Guardrails
- Hallucination Detection
- LLM
- Agents
---
