---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: carmax.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.carmax.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carmax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarMax, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CarMax
provider_slug: carmax
slug: carmax-domain-security
source_filename: carmax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carmax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: carmax.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carmax/refs/heads/main/security/carmax-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Auto Financing
- Auto Retail
- Appraisals
- Automotive
- Omnichannel
- Retail
- Server-Driven UI
- Used Cars
- Vehicle Inventory
- VIN Lookup
- Fortune 500
---
