---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sleekev.com
  spf: true
hosts:
- cert_expires: Sep  8 23:09:37 2026 GMT
  host: sleekev.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sleek Ev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sleek EV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sleek EV
provider_slug: sleek-ev
slug: sleek-ev-domain-security
source_filename: sleek-ev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sleekev.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 23:09:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sleekev.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleek-ev/refs/heads/main/security/sleek-ev-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Electric Vehicles
- Electric Motorcycles
- EV Charging
- Sustainability
- Mobility
- Thailand
- Southeast Asia
---
