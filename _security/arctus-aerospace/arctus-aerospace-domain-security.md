---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: arctus.space
  spf: true
hosts:
- cert_expires: Sep 19 02:17:00 2026 GMT
  host: arctus.space
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arctus Aerospace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arctus Aerospace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Arctus Aerospace
provider_slug: arctus-aerospace
slug: arctus-aerospace-domain-security
source_filename: arctus-aerospace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arctus.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:17:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: arctus.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arctus-aerospace/refs/heads/main/security/arctus-aerospace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Deep Tech
- Aerospace
- Earth Observation
- Geospatial
- Unmanned Aircraft
- Defense
- Data as a Service
---
