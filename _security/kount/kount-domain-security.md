---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kount.com
  spf: true
hosts:
- cert_expires: Sep 15 11:51:28 2026 GMT
  host: kount.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 23:45:53 2026 GMT
  host: developer.kount.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: api.kount.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kount Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kount, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kount
provider_slug: kount
slug: kount-domain-security
source_filename: kount-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 11:51:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.kount.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:45:53 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.kount.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: kount.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kount/refs/heads/main/security/kount-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Fraud Detection
- Chargebacks
- Payments
- Identity
- Risk Scoring
- Device Intelligence
- Account Takeover
---
