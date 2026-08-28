---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vynaris.com
  spf: true
hosts:
- cert_expires: Oct 22 09:03:27 2026 GMT
  host: vynaris.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:37:19 2026 GMT
  host: api.vynaris.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vynaris Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vynaris, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vynaris
provider_slug: vynaris
slug: vynaris-domain-security
source_filename: vynaris-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vynaris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 09:03:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.vynaris.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:37:19 2026 GMT\n  hsts: null\ndomains:\n- domain: vynaris.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vynaris/refs/heads/main/security/vynaris-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM Gateway
- LLM Router / Aggregator
- Inference / Model Serving
- AI Cost Management / FinOps
- Developer Tools
- Agent Infrastructure
---
