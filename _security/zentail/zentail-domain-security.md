---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zentail.com
  spf: true
hosts:
- cert_expires: Sep 16 20:25:38 2026 GMT
  host: developer.zentail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 12:04:45 2026 GMT
  host: api.zentail.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zentail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zentail, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zentail
provider_slug: zentail
slug: zentail-domain-security
source_filename: zentail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.zentail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 20:25:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.zentail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 12:04:45 2026 GMT\n  hsts: null\ndomains:\n- domain: zentail.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zentail/refs/heads/main/security/zentail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ecommerce
- Multichannel
- Marketplace
- Product Information Management
- Inventory Management
- Order Management
- Listing Management
- Retail
---
