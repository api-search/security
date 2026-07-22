---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eloquii.com
  spf: true
hosts:
- cert_expires: Nov 30 20:01:37 2026 GMT
  host: eloquii.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Eloquii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eloquii, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eloquii
provider_slug: eloquii
slug: eloquii-domain-security
source_filename: eloquii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eloquii.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 30 20:01:37 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: eloquii.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eloquii/refs/heads/main/security/eloquii-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Retail
- Ecommerce
- Fashion
- Apparel
- Plus Size
- Direct to Consumer
- Consumer
---
