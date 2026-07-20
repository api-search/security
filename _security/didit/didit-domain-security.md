---
api_specs:
- filename: didit-openapi-original.json
  format: json
  label: Didit Verification API
  slug: didit-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/openapi/didit-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: didit.me
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: verification.didit.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Didit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Didit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Didit
provider_slug: didit
slug: didit-domain-security
source_filename: didit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verification.didit.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: didit.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/didit/refs/heads/main/security/didit-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Identity
- Identity Verification
- KYC
- KYB
- AML
- Fraud Prevention
- Compliance
- Biometrics
- Transaction Monitoring
- Crypto
---
