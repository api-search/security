---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: condoit.io
  spf: true
hosts:
- cert_expires: Oct  5 19:45:34 2026 GMT
  host: condoit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Condoit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Con.doit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Con.doit
provider_slug: condoit
slug: condoit-domain-security
source_filename: condoit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: condoit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:45:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: condoit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/condoit/refs/heads/main/security/condoit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electrical
- Contractors
- Field Service
- Facility Management
- Thermography
- NFPA 70B
- Asset Management
- Compliance
---
