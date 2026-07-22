---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tem.energy
  spf: true
hosts:
- cert_expires: Sep  1 23:20:44 2026 GMT
  host: tem.energy
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: api.tem.energy
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tem, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tem
provider_slug: tem
slug: tem-domain-security
source_filename: tem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tem.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:20:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tem.energy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tem.energy\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tem/refs/heads/main/security/tem-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Electricity
- Utilities
- Sustainability
- Renewable Energy
- Fintech
- Infrastructure
- United Kingdom
---
