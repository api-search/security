---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: shuftipro.com
  spf: true
hosts:
- cert_expires: Aug 29 08:45:16 2026 GMT
  host: shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 28 09:40:26 2026 GMT
  host: developers.shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 18:59:52 2026 GMT
  host: api.shuftipro.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shufti Pro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shufti Pro, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Shufti Pro
provider_slug: shufti-pro
slug: shufti-pro-domain-security
source_filename: shufti-pro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 08:45:16 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: developers.shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 09:40:26 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.shuftipro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:59:52 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: shuftipro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shufti-pro/refs/heads/main/security/shufti-pro-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- KYC
- AML
- KYB
- Face Biometrics
- Document Verification
- Address Verification
- Liveness Detection
- eIDV
- Compliance
- Fraud Prevention
---
