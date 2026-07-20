---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cognitohq.com
  spf: true
hosts:
- cert_expires: Sep 28 10:40:18 2026 GMT
  host: cognitohq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: api.cognitohq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cognito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognito, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cognito
provider_slug: cognito
slug: cognito-domain-security
source_filename: cognito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognitohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 10:40:18 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.cognitohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: cognitohq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognito/refs/heads/main/security/cognito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Identity
- Identity Verification
- KYC
- AML
- Compliance
- Fraud Prevention
- Onboarding
- Watchlist Screening
- Know Your Customer
---
