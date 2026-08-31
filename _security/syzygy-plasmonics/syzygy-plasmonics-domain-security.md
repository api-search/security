---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plasmonics.tech
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: www.plasmonics.tech
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Syzygy Plasmonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Syzygy Plasmonics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Syzygy Plasmonics
provider_slug: syzygy-plasmonics
slug: syzygy-plasmonics-domain-security
source_filename: syzygy-plasmonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plasmonics.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: plasmonics.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/syzygy-plasmonics/refs/heads/main/security/syzygy-plasmonics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Cleantech
- Hydrogen
- Sustainable Aviation Fuel
- Chemicals
- Decarbonization
- Manufacturing
- Photocatalysis
---
