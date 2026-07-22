---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tebi.co
  spf: true
hosts:
- cert_expires: Oct 16 10:27:03 2026 GMT
  host: tebi.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tebi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tebi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tebi
provider_slug: tebi
slug: tebi-domain-security
source_filename: tebi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tebi.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 10:27:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tebi.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tebi/refs/heads/main/security/tebi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Point of Sale
- Hospitality
- Restaurants
- Reservations
- Inventory
- CRM
---
