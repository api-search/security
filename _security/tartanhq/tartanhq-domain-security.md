---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tartanhq.com
  spf: true
hosts:
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: tartanhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tartanhq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TartanHQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TartanHQ
provider_slug: tartanhq
slug: tartanhq-domain-security
source_filename: tartanhq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tartanhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tartanhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tartanhq/refs/heads/main/security/tartanhq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Verification
- Identity
- KYC
- KYB
- Financial Services
- Insurance
- HR Tech
- Lending
- API Infrastructure
- Fintech
- India
---
