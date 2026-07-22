---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mwivet.com
  spf: true
hosts:
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: www.mwivet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mwi Veterinary Supply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MWI Veterinary Supply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MWI Veterinary Supply
provider_slug: mwi-veterinary-supply
slug: mwi-veterinary-supply-domain-security
source_filename: mwi-veterinary-supply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mwivet.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mwivet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mwi-veterinary-supply/refs/heads/main/security/mwi-veterinary-supply-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Animal Health
- Distribution
- Pharmaceuticals
- Veterinary
- Veterinary Supply
---
