---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: altair-semi.com
  spf: true
hosts:
- cert_expires: Sep  5 13:03:08 2026 GMT
  host: altair-semi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altair Semiconductor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altair Semiconductor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Altair Semiconductor
provider_slug: altair-semiconductor
slug: altair-semiconductor-domain-security
source_filename: altair-semiconductor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altair-semi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 13:03:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: altair-semi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altair-semiconductor/refs/heads/main/security/altair-semiconductor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Semiconductor
- Cellular IoT
- Chipset
- LPWA
- NB-IoT
- LTE-M
- 5G
- Deep Tech
---
