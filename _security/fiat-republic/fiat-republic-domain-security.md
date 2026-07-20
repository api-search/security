---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fiatrepublic.com
  spf: true
hosts:
- cert_expires: Sep 29 10:08:41 2026 GMT
  host: fiatrepublic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:42:13 2026 GMT
  host: docs.fiatrepublic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 10:08:41 2026 GMT
  host: member.fiatrepublic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fiat Republic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fiat Republic, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Fiat Republic
provider_slug: fiat-republic
slug: fiat-republic-domain-security
source_filename: fiat-republic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiatrepublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fiatrepublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: member.fiatrepublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:08:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fiatrepublic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiat-republic/refs/heads/main/security/fiat-republic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Payments
- Fintech
- Cryptocurrency
- Stablecoins
- Banking-as-a-Service
- Embedded Finance
- Compliance
- KYC
- SEPA
- Faster Payments
---
