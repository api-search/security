---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tatio.io
  spf: true
hosts:
- cert_expires: Aug 12 16:48:29 2026 GMT
  host: tatio.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tatio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TaTiO, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TaTiO
provider_slug: tatio
slug: tatio-domain-security
source_filename: tatio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tatio.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:48:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: tatio.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tatio/refs/heads/main/security/tatio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hiring
- Recruitment
- Candidate Assessment
- Job Simulations
- Human Resources
- Talent
- MCP
---
