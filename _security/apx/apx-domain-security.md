---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apx.group
  spf: true
hosts:
- cert_expires: Sep 27 21:02:24 2026 GMT
  host: apx.group
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Apx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: APX
provider_slug: apx
slug: apx-domain-security
source_filename: apx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apx.group\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 21:02:24 2026 GMT\n  hsts: false\ndomains:\n- domain: apx.group\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apx/refs/heads/main/security/apx-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Logistics
- Shipping
- Freight
- Supply Chain
- Southeast Asia
- Transportation
- Customs
- Warehousing
---
