---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thisisaday.com
  spf: true
hosts:
- cert_expires: Aug 27 08:02:02 2026 GMT
  host: thisisaday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aday Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aday, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aday
provider_slug: aday
slug: aday-domain-security
source_filename: aday-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thisisaday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 08:02:02 2026 GMT\n  hsts: null\ndomains:\n- domain: thisisaday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aday/refs/heads/main/security/aday-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Fashion
- Apparel
- Ecommerce
- Sustainability
- Direct to Consumer
- Retail
- Shopify
---
