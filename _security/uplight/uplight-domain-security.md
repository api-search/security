---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uplight.com
  spf: true
hosts:
- cert_expires: Oct 22 17:33:31 2026 GMT
  host: uplight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:06:36 2026 GMT
  host: docs.uplight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 14:51:33 2026 GMT
  host: api.uplight.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uplight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uplight, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Uplight
provider_slug: uplight
slug: uplight-domain-security
source_filename: uplight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uplight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 17:33:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.uplight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.uplight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:51:33 2026 GMT\n  hsts: null\ndomains:\n- domain: uplight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uplight/refs/heads/main/security/uplight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Utilities
- Electricity
- Gas
- Demand Response
- DER
- Grid
- Virtual Power Plant
- DERMS
- Energy Efficiency
- Customer Engagement
---
