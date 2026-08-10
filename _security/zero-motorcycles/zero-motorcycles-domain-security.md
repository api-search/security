---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeromotorcycles.com
  spf: true
hosts:
- cert_expires: Sep 13 16:23:47 2026 GMT
  host: zeromotorcycles.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zero Motorcycles Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zero Motorcycles, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zero Motorcycles
provider_slug: zero-motorcycles
slug: zero-motorcycles-domain-security
source_filename: zero-motorcycles-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeromotorcycles.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 16:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zeromotorcycles.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zero-motorcycles/refs/heads/main/security/zero-motorcycles-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Electric Vehicles
- Motorcycles
- Automotive
- Manufacturing
- Connected Vehicles
- Telematics
- Mobility
---
