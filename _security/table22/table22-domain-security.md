---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: table22.com
  spf: true
hosts:
- cert_expires: Oct  5 22:55:20 2026 GMT
  host: www.table22.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Table22 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Table22, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Table22
provider_slug: table22
slug: table22-domain-security
source_filename: table22-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.table22.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 22:55:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: table22.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/table22/refs/heads/main/security/table22-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Subscription Commerce
- Food and Beverage
- Hospitality
- Ecommerce
- Memberships
- Recurring Revenue
- Wine Clubs
- Fulfillment
---
