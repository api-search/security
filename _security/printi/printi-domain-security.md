---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: printi.com.br
  spf: true
hosts:
- cert_expires: Oct  8 05:32:17 2026 GMT
  host: www.printi.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Printi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Printi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Printi
provider_slug: printi
slug: printi-domain-security
source_filename: printi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.printi.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 05:32:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: printi.com.br\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printi/refs/heads/main/security/printi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Printing
- Print on Demand
- Commercial Print
- Marketplace
- Ecommerce
- Brazil
- Cimpress
- Partner Gated
---
