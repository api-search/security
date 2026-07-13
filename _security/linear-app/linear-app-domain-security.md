---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: linear.app
  spf: true
hosts:
- cert_expires: Oct  6 22:29:55 2026 GMT
  host: linear.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linear App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linear, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Linear
provider_slug: linear-app
slug: linear-app-domain-security
source_filename: linear-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linear.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 22:29:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: linear.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linear-app/refs/heads/main/security/linear-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Project Management
- Issue Tracking
- Productivity
- SaaS
- GraphQL
- Developer Tools
- Agents
---
