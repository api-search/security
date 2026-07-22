---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: molsoncoors.com
  spf: true
hosts:
- cert_expires: Oct  3 06:13:50 2026 GMT
  host: www.molsoncoors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Molson Coors Beverage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Molson Coors Beverage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Molson Coors Beverage
provider_slug: molson-coors-beverage
slug: molson-coors-beverage-domain-security
source_filename: molson-coors-beverage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.molsoncoors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: molsoncoors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/molson-coors-beverage/refs/heads/main/security/molson-coors-beverage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 500
- Beverages
- Brewing
---
