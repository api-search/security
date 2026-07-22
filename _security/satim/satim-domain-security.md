---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: satim.co
  spf: true
hosts:
- cert_expires: Oct 15 03:33:49 2026 GMT
  host: satim.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Satim Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SATIM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SATIM
provider_slug: satim
slug: satim-domain-security
source_filename: satim-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: satim.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 03:33:49 2026 GMT\n  hsts: false\ndomains:\n- domain: satim.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/satim/refs/heads/main/security/satim-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Defense
- Intelligence
- Geospatial
- Synthetic Aperture Radar
- Satellite Imagery
- Artificial Intelligence
- ISR
---
