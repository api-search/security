---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aimon.ai
  spf: true
hosts:
- cert_expires: Oct  7 19:51:35 2026 GMT
  host: www.aimon.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:21:02 2026 GMT
  host: docs.aimon.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: sdkbe-production.aimon.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Aimon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIMon, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AIMon
provider_slug: aimon
slug: aimon-domain-security
source_filename: aimon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aimon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 19:51:35 2026 GMT\n  hsts: false\n- host: docs.aimon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:21:02 2026 GMT\n  hsts: false\n- host: sdkbe-production.aimon.ai\n  https: false\ndomains:\n- domain: aimon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aimon/refs/heads/main/security/aimon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai Ml
- LLM Observability
- AI Monitoring
- Evaluation
- Hallucination Detection
- LLM Guardrails
- RAG
- AI Governance
- Trustworthy AI
---
