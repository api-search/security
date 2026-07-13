---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: craftable.com
  spf: true
hosts:
- cert_expires: Aug 24 14:05:10 2026 GMT
  host: craftable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Craftable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Craftable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Craftable
provider_slug: craftable
slug: craftable-domain-security
source_filename: craftable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: craftable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 14:05:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: craftable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/craftable/refs/heads/main/security/craftable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Back Office
- Inventory
- Procurement
- Invoices
- Accounting
- Hospitality
- Recipe Management
- Accounts Payable
- Point Of Sale
---
