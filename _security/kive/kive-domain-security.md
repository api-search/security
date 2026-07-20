---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kive.ai
  spf: true
hosts:
- cert_expires: Oct 13 01:42:29 2026 GMT
  host: www.kive.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kive
provider_slug: kive
slug: kive-domain-security
source_filename: kive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 01:42:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kive.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kive/refs/heads/main/security/kive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SaaS
- Artificial Intelligence
- Generative AI
- Creative
- Product Photography
- Digital Asset Management
- E-Commerce
- Images
- Video
- MCP
---
