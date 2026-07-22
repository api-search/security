---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: warehousing1.com
  spf: true
hosts:
- cert_expires: Sep 21 05:55:56 2026 GMT
  host: warehousing1.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warehousing1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warehousing1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Warehousing1
provider_slug: warehousing1
slug: warehousing1-domain-security
source_filename: warehousing1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: warehousing1.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 05:55:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: warehousing1.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warehousing1/refs/heads/main/security/warehousing1-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fulfillment
- Warehousing
- Logistics
- E-Commerce
- Supply Chain
- 3PL
- Marketplace
- Germany
---
