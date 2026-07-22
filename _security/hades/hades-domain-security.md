---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hades.com
  spf: true
hosts:
- cert_expires: Sep  4 22:02:07 2026 GMT
  host: www.hades.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hades Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hades, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Hades
provider_slug: hades
slug: hades-domain-security
source_filename: hades-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hades.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 22:02:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hades.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hades/refs/heads/main/security/hades-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Deep Tech
- Mining
- Critical Minerals
- Geothermal Energy
- Laser Drilling
- In-Situ Recovery
- Energy
- Germany
---
