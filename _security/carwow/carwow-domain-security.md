---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carwow.co.uk
  spf: true
hosts:
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: www.carwow.co.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Carwow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carwow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carwow
provider_slug: carwow
slug: carwow-domain-security
source_filename: carwow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carwow.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: carwow.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carwow/refs/heads/main/security/carwow-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Automotive
- Marketplace
- Car Buying
- Car Selling
- Leasing
- Electric Vehicles
- United Kingdom
---
