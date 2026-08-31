---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prizeout.com
  spf: true
hosts:
- cert_expires: Oct 13 06:30:08 2026 GMT
  host: www.prizeout.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 16:57:17 2026 GMT
  host: candidate.prizeout.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 16:57:17 2026 GMT
  host: widget-v2.prizeout.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prizeout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prizeout, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prizeout
provider_slug: prizeout
slug: prizeout-domain-security
source_filename: prizeout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prizeout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:30:08 2026 GMT\n  hsts: false\n- host: candidate.prizeout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 16:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: widget-v2.prizeout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 16:57:17 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: prizeout.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prizeout/refs/heads/main/security/prizeout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Rewards
- Gift Cards
- Payouts
- Financial-Services
- Credit Unions
- Banking
- Loyalty
- Embedded Finance
- AdTech
- Fintech
---
