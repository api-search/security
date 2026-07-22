---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: picogrid.com
  spf: true
hosts:
- cert_expires: Sep  9 17:38:15 2026 GMT
  host: picogrid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:12:45 2026 GMT
  host: docs.picogrid.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: legion-prod.picogrid.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Picogrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Picogrid, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Picogrid
provider_slug: picogrid
slug: picogrid-domain-security
source_filename: picogrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: picogrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 17:38:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.picogrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 15:12:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: legion-prod.picogrid.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: picogrid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picogrid/refs/heads/main/security/picogrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Data
- Defense
- Public Safety
- Systems Integration
- Sensors
- Unmanned Systems
- Command and Control
- Geospatial
- Situational Awareness
- OAuth
- Video Streaming
---
