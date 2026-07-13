---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dutchie.com
  spf: true
hosts:
- cert_expires: Oct  9 15:29:17 2026 GMT
  host: dutchie.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 01:29:14 2026 GMT
  host: plus.dutchie.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dutchie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dutchie, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Dutchie
provider_slug: dutchie
slug: dutchie-domain-security
source_filename: dutchie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dutchie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:29:17 2026 GMT\n  hsts: false\n- host: plus.dutchie.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 01:29:14 2026 GMT\n  hsts: null\ndomains:\n- domain: dutchie.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dutchie/refs/heads/main/security/dutchie-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cannabis
- Dispensary
- Retail
- Ecommerce
- Point of Sale
- Headless Commerce
- GraphQL
- Menu
- Checkout
---
