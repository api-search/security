---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: revelsystems.com
  spf: true
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: revelsystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 10:44:08 2026 GMT
  host: developer.revelsystems.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Revel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Revel Systems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Revel Systems
provider_slug: revel
slug: revel-domain-security
source_filename: revel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: revelsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\n- host: developer.revelsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 10:44:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: revelsystems.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revel/refs/heads/main/security/revel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- POS
- Point of Sale
- Restaurant
- Retail
- iPad
- Orders
- Inventory
- Loyalty
- Payments
---
