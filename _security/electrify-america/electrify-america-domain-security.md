---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: electrifyamerica.com
  spf: true
hosts:
- cert_expires: Sep 27 16:42:50 2026 GMT
  host: www.electrifyamerica.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 16:42:50 2026 GMT
  host: developer.electrifyamerica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: api.electrifyamerica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Electrify America Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Electrify America, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Electrify America
provider_slug: electrify-america
slug: electrify-america-domain-security
source_filename: electrify-america-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.electrifyamerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.electrifyamerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 16:42:50 2026 GMT\n  hsts: null\n- host: api.electrifyamerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: electrifyamerica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electrify-america/refs/heads/main/security/electrify-america-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Electric Vehicles
- EV Charging
- Charging Stations
- DC Fast Charging
- Plug and Charge
- Automotive
- Energy
- Transportation
- Mobility
---
