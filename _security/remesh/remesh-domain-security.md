---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remesh.ai
  spf: true
hosts:
- cert_expires: Aug 19 18:12:21 2026 GMT
  host: remesh.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remesh, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Remesh
provider_slug: remesh
slug: remesh-domain-security
source_filename: remesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: remesh.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 18:12:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: remesh.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remesh/refs/heads/main/security/remesh-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Market Research
- Insights
- Artificial Intelligence
- Employee Listening
- Focus Groups
- SaaS
---
