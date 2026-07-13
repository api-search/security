---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cantaloupe.com
  spf: true
hosts:
- cert_expires: Aug 25 18:11:30 2026 GMT
  host: www.cantaloupe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cantaloupe Seed Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cantaloupe Seed API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cantaloupe Seed API
provider_slug: cantaloupe-seed-api
slug: cantaloupe-seed-api-domain-security
source_filename: cantaloupe-seed-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cantaloupe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:11:30 2026 GMT\n  hsts: false\ndomains:\n- domain: cantaloupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cantaloupe-seed-api/refs/heads/main/security/cantaloupe-seed-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Billing
- Cashless Payments
- Micro Markets
- Office Coffee
- Payments
- Retail
- Self-Service Retail
- Unattended Retail
- Vending
---
