---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: storehub.com
  spf: true
hosts:
- cert_expires: Sep 18 01:31:59 2026 GMT
  host: storehub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storehub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StoreHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: StoreHub
provider_slug: storehub
slug: storehub-domain-security
source_filename: storehub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: storehub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 01:31:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: storehub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storehub/refs/heads/main/security/storehub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Point of Sale
- Retail
- Restaurant
- Inventory Management
- Payments
- E-commerce
- Loyalty
- Southeast Asia
- Small Business
---
