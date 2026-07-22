---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: actualyze.ai
  spf: true
hosts:
- cert_expires: Oct  3 01:03:01 2026 GMT
  host: actualyze.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Actualyzeai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Actualyze AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Actualyze AI
provider_slug: actualyzeai
slug: actualyzeai-domain-security
source_filename: actualyzeai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: actualyze.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:03:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: actualyze.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actualyzeai/refs/heads/main/security/actualyzeai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- AI Governance
- Enterprise AI
- Compliance
- Security
- Machine Learning
- Observability
---
