---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: wallex.asia
  spf: true
hosts:
- cert_expires: Oct 12 06:03:04 2026 GMT
  host: wallex.asia
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wallex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wallex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Wallex
provider_slug: wallex
slug: wallex-domain-security
source_filename: wallex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wallex.asia\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 06:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: wallex.asia\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wallex/refs/heads/main/security/wallex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Payments
- Cross-Border Payments
- Foreign Exchange
- Fintech
- Collections
- B2B Payments
- Embedded Finance
- Southeast Asia
---
