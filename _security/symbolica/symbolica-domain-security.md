---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: symbolica.ai
  spf: true
hosts:
- cert_expires: Sep 12 16:35:46 2026 GMT
  host: www.symbolica.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Symbolica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symbolica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Symbolica
provider_slug: symbolica
slug: symbolica-domain-security
source_filename: symbolica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.symbolica.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 16:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: symbolica.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symbolica/refs/heads/main/security/symbolica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Agents
- Agentic AI
- SDK
- Developer Tools
- LLM
- Machine Learning
---
