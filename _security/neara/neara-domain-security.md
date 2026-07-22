---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: neara.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: neara.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Neara
provider_slug: neara
slug: neara-domain-security
source_filename: neara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: neara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: neara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neara/refs/heads/main/security/neara-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Utilities
- Energy
- Digital Twin
- Electricity Grid
- LiDAR
- GIS
- Simulation
- Wildfire Mitigation
- Vegetation Management
- Asset Management
- Infrastructure
---
