---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sunfire.de
  spf: true
hosts:
- cert_expires: Nov 15 12:42:40 2026 GMT
  host: sunfire.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sunfire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sunfire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sunfire
provider_slug: sunfire
slug: sunfire-domain-security
source_filename: sunfire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sunfire.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 12:42:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sunfire.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sunfire/refs/heads/main/security/sunfire-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Green Hydrogen
- Electrolysis
- Power-to-X
- Renewable Energy
- Industrial Manufacturing
- Hydrogen Technology
- Synthetic Fuels
- Germany
---
