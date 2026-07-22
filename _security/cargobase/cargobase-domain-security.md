---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cargobase.com
  spf: true
hosts:
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: cargobase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cargobase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cargobase, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cargobase
provider_slug: cargobase
slug: cargobase-domain-security
source_filename: cargobase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cargobase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: cargobase.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cargobase/refs/heads/main/security/cargobase-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Logistics
- Transportation Management System
- Freight
- Supply Chain
- Spot Freight
- Freight Procurement
- Shipping
---
