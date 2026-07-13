---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lexisnexis.com
  spf: true
hosts:
- cert_expires: Apr 11 14:51:24 2027 GMT
  host: www.lexisnexis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 22 11:42:16 2026 GMT
  host: dev.lexisnexis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 11 21:06:20 2026 GMT
  host: risk.lexisnexis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lexisnexis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LexisNexis, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LexisNexis
provider_slug: lexisnexis
slug: lexisnexis-domain-security
source_filename: lexisnexis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lexisnexis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 11 14:51:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: dev.lexisnexis.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 11:42:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: risk.lexisnexis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 21:06:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lexisnexis.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lexisnexis/refs/heads/main/security/lexisnexis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal
- Risk
- Identity Verification
- Fraud Detection
- Compliance
- Analytics
- Data
---
