---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: provi.com
  spf: true
hosts:
- cert_expires: Sep  4 14:11:14 2026 GMT
  host: www.provi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Provi
provider_slug: provi
slug: provi-domain-security
source_filename: provi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.provi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 14:11:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: provi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provi/refs/heads/main/security/provi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beverage
- Alcohol
- Marketplace
- B2B
- E-commerce
- Distribution
- Hospitality
---
