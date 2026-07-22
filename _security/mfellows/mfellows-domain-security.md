---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: moneyfellows.com
  spf: true
hosts:
- cert_expires: Oct  7 13:59:25 2026 GMT
  host: moneyfellows.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mfellows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MFellows, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: MFellows
provider_slug: mfellows
slug: mfellows-domain-security
source_filename: mfellows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moneyfellows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 13:59:25 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: moneyfellows.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mfellows/refs/heads/main/security/mfellows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Financial Services
- Savings
- Lending
- ROSCA
- Payments
- Egypt
- Mobile
- Consumer Finance
---
