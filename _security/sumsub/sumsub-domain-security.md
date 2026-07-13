---
api_specs:
- filename: PostmanCollection
  format: yaml
  label: Sumsub API
  slug: sumsub-api
  spec_type: Postman
  url: https://github.com/SumSubstance/PostmanCollection
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sumsub.com
  spf: true
hosts:
- cert_expires: Oct  9 11:06:46 2026 GMT
  host: sumsub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 10:32:33 2026 GMT
  host: docs.sumsub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 03:33:56 2026 GMT
  host: api.sumsub.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sumsub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sumsub, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sumsub
provider_slug: sumsub
slug: sumsub-domain-security
source_filename: sumsub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sumsub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 11:06:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.sumsub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 10:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sumsub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 03:33:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sumsub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumsub/refs/heads/main/security/sumsub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AML
- Compliance
- Fraud Prevention
- Identity Verification
- KYB
- KYC
- Transaction Monitoring
- Travel Rule
---
