---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tala.co
  spf: true
hosts:
- cert_expires: Sep  2 21:51:41 2026 GMT
  host: tala.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tala Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tala, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tala
provider_slug: tala
slug: tala-domain-security
source_filename: tala-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tala.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 21:51:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tala.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tala/refs/heads/main/security/tala-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Credit
- Digital Wallet
- Mobile
- Embedded Finance
- Consumer Finance
- Emerging Markets
---
