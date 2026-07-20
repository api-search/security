---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: superpenguin.ai
  spf: true
hosts:
- cert_expires: Sep  6 23:05:59 2026 GMT
  host: superpenguin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 23:05:59 2026 GMT
  host: app.superpenguin.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carrot Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carrot Labs, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Carrot Labs
provider_slug: carrot-labs
slug: carrot-labs-domain-security
source_filename: carrot-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superpenguin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.superpenguin.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:05:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: superpenguin.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carrot-labs/refs/heads/main/security/carrot-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- FinOps
- AIOps
- Cost Management
- LLM
- Observability
- Developer Tools
---
