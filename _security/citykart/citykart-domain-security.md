---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: citykart.co.in
  spf: true
hosts:
- cert_expires: Nov 19 11:56:32 2026 GMT
  host: citykart.co.in
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Citykart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citykart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Citykart
provider_slug: citykart
slug: citykart-domain-security
source_filename: citykart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: citykart.co.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 11:56:32 2026 GMT\n  hsts: false\ndomains:\n- domain: citykart.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citykart/refs/heads/main/security/citykart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fashion Retail
- Apparel
- Footwear
- Accessories
- Home Essentials
- Family Shopping
- Indian Market
---
