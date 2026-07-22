---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: openlightphotonics.com
  spf: true
hosts:
- cert_expires: Sep  2 12:33:51 2026 GMT
  host: openlightphotonics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openlight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openlight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Openlight
provider_slug: openlight
slug: openlight-domain-security
source_filename: openlight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openlightphotonics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 12:33:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openlightphotonics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlight/refs/heads/main/security/openlight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Silicon Photonics
- Semiconductors
- Photonics
- PASIC
- Hardware
- Data Center
- Optical Interconnect
- Chip Design
- Deep Tech
---
