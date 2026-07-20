---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jasper.ai
  spf: true
hosts:
- cert_expires: Sep 13 01:03:28 2026 GMT
  host: www.jasper.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:55:51 2026 GMT
  host: developers.jasper.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 13:49:10 2026 GMT
  host: api.jasper.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jasper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jasper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jasper
provider_slug: jasper
slug: jasper-domain-security
source_filename: jasper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 01:03:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:55:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 13:49:10 2026 GMT\n  hsts: null\ndomains:\n- domain: jasper.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jasper/refs/heads/main/security/jasper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Artificial Intelligence
- Content Generation
- Marketing
- Generative AI
- Agents
- MCP
---
