---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inertia.com
  spf: true
hosts:
- cert_expires: Sep  7 01:34:07 2026 GMT
  host: inertia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inertia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inertia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inertia
provider_slug: inertia
slug: inertia-domain-security
source_filename: inertia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inertia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 01:34:07 2026 GMT\n  hsts: false\ndomains:\n- domain: inertia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inertia/refs/heads/main/security/inertia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
- Fusion Energy
- Clean Energy
- Inertial Confinement Fusion
- Laser
- Power Generation
- Climate Tech
---
