---
description: ''
domains:
- caa: []
  dmarc: true
  dnssec: false
  domain: akur8.com
  spf: true
hosts:
- cert_expires: Aug 16 18:28:12 2026 GMT
  host: www.akur8.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akur8 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akur8, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present.'
provider_name: Akur8
provider_slug: akur8
slug: akur8-domain-security
source_filename: akur8-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akur8.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:28:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akur8.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akur8/refs/heads/main/security/akur8-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Actuarial
- Pricing
- GLM
- Rating Engine
---
