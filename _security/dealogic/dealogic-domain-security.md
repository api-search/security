---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dealogic.com
  spf: true
hosts:
- cert_expires: Sep 13 22:41:46 2026 GMT
  host: www.dealogic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dealogic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dealogic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dealogic
provider_slug: dealogic
slug: dealogic-domain-security
source_filename: dealogic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dealogic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:41:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dealogic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealogic/refs/heads/main/security/dealogic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Capital Markets
- Compliance
- Deal Management
- Finance
- Financial Data
- Investment Banking
- League Tables
---
