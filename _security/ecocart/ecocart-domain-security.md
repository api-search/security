---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ecocart.io
  spf: true
hosts:
- cert_expires: Sep 23 16:08:51 2026 GMT
  host: ecocart.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: dev.ecocart.io
  https: false
- host: api.ecocart.io
  https: false
kind: domain-security
layout: security
method: probed
name: Ecocart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EcoCart, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EcoCart
provider_slug: ecocart
slug: ecocart-domain-security
source_filename: ecocart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecocart.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:08:51 2026 GMT\n  hsts: false\n- host: dev.ecocart.io\n  https: false\n- host: api.ecocart.io\n  https: false\ndomains:\n- domain: ecocart.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecocart/refs/heads/main/security/ecocart-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sustainability
- Carbon Offsets
- E-commerce
- Climate
- Checkout
- Shipping Protection
- Returns
---
