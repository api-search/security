---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withclutch.com
  spf: true
hosts:
- cert_expires: Sep 28 02:13:50 2026 GMT
  host: withclutch.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 18:38:44 2026 GMT
  host: support.withclutch.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Withclutch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clutch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clutch
provider_slug: withclutch
slug: withclutch-domain-security
source_filename: withclutch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withclutch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 02:13:50 2026 GMT\n  hsts: false\n- host: support.withclutch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 18:38:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withclutch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withclutch/refs/heads/main/security/withclutch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Credit Unions
- Lending
- Loan Origination
- Account Opening
- Financial-Services
- Fintech
- Banking
- Data Exports
---
