---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cantaloupe.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: seedlive.com
  note: No SPF TXT, no _dmarc record, no CAA, no DS. Probed by hand 2026-08-28.
  spf: false
hosts:
- cert_expires: Oct 24 00:09:27 2026 GMT
  host: www.cantaloupe.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: seedlive.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Seed Live customer portal, Cantaloupe-operated. Probed by hand 2026-08-28; not reachable from apis.yml hosts because Cantaloupe publishes no Seed API base URL.
- host: api.seedlive.com
  hsts: false
  https: true
  note: AWS API Gateway. HTTP 403 {"message":"Missing Authentication Token"} on every path. No HSTS header on the anonymous response.
kind: domain-security
layout: security
method: probed
name: Seed Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Seed, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Seed
provider_slug: seed-platform
slug: seed-platform-domain-security
source_filename: seed-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cantaloupe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 00:09:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: seedlive.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  note: >-\n    Seed Live customer portal, Cantaloupe-operated. Probed by hand 2026-08-28;\n    not reachable from apis.yml hosts because Cantaloupe publishes no Seed API\n    base URL.\n- host: api.seedlive.com\n  https: true\n  hsts: false\n  note: >-\n    AWS API Gateway. HTTP 403 {\"message\":\"Missing Authentication Token\"} on every\n    path. No HSTS header on the anonymous response.\ndomains:\n- domain: cantaloupe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: seedlive.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  note: >-\n    No SPF TXT,\
  \ no _dmarc record, no CAA, no DS. Probed by hand 2026-08-28.\nx-hand-probes:\n  date: '2026-08-28'\n  note: >-\n    The seedlive.com and api.seedlive.com rows were added by the enrichment pass,\n    not by probe-domain-security.py, which reads only apis.yml baseURL/servers\n    hosts and this provider publishes no base URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seed-platform/refs/heads/main/security/seed-platform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Cashless Payments
- Vending
- Micro Markets
- Unattended Retail
- Self-Service Retail
- Point of Sale
- Sales Reporting
- Billing
- Office Coffee
---
