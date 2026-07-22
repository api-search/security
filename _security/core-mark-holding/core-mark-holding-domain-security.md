---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: core-mark.com
  spf: true
hosts:
- cert_expires: Aug 14 23:59:59 2026 GMT
  host: www.core-mark.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Core Mark Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Core-Mark Holding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Core-Mark Holding
provider_slug: core-mark-holding
slug: core-mark-holding-domain-security
source_filename: core-mark-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.core-mark.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: core-mark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/core-mark-holding/refs/heads/main/security/core-mark-holding-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Beverages
- Candy
- Consumer Packaged Goods
- Convenience Stores
- Distribution
- Foodservice
- Logistics
- Retail
- Snacks
- Tobacco
- Wholesale
- Fortune 500
---
