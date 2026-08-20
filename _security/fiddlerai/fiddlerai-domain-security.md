---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fiddler.ai
  spf: true
hosts:
- cert_expires: Oct 14 23:20:08 2026 GMT
  host: www.fiddler.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 31 22:41:33 2026 GMT
  host: docs.fiddler.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 22 03:37:51 2026 GMT
  host: demo.fiddler.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Fiddlerai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fiddler.ai, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: fiddler.ai
provider_slug: fiddlerai
slug: fiddlerai-domain-security
source_filename: fiddlerai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fiddler.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 14 23:20:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fiddler.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 31 22:41:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: demo.fiddler.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 22 03:37:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: fiddler.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiddlerai/refs/heads/main/security/fiddlerai-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- AI Observability
- Machine-Learning
- LLM
- Model Monitoring
- Guardrails
- MLOps
- AI Governance
- Explainability
- Agent Observability
- AI Security
---
