---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tsm.gg
  spf: false
hosts:
- cert_expires: Oct  6 16:31:07 2026 GMT
  host: www.tsm.gg
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tsm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TSM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: TSM
provider_slug: tsm
slug: tsm-domain-security
source_filename: tsm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tsm.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 16:31:07 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: tsm.gg\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsm/refs/heads/main/security/tsm-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Consumer
- Esports
- Gaming
- Ecommerce
- Merchandise
- Retail
---
