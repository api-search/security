---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: retailmenot.com
  spf: true
hosts:
- cert_expires: Oct 15 13:31:18 2026 GMT
  host: retailmenot.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Retailmenot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RetailMeNot *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RetailMeNot *
provider_slug: retailmenot
slug: retailmenot-domain-security
source_filename: retailmenot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: retailmenot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 13:31:18 2026 GMT\n  hsts: null\ndomains:\n- domain: retailmenot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/retailmenot/refs/heads/main/security/retailmenot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Coupons
- Deals
- Cashback
- Savings
- Shopping
- Retail
- Ecommerce
---
