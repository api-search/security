---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: matter.com
  spf: true
hosts:
- cert_expires: Nov 21 00:28:15 2026 GMT
  host: www.matter.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matter Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matter Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Matter Intelligence
provider_slug: matter-intelligence
slug: matter-intelligence-domain-security
source_filename: matter-intelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.matter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 00:28:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: matter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matter-intelligence/refs/heads/main/security/matter-intelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Remote Sensing
- Earth Observation
- Hyperspectral Imaging
- Geospatial
- Satellite Imagery
- Sensors
- Artificial Intelligence
- Climate
- Aerospace
---
