---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: signifyd.com
  spf: true
hosts:
- cert_expires: Sep 15 20:13:47 2026 GMT
  host: www.signifyd.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:51:41 2026 GMT
  host: developer.signifyd.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signifyd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Signifyd, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Signifyd
provider_slug: signifyd
slug: signifyd-domain-security
source_filename: signifyd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.signifyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.signifyd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:51:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signifyd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signifyd/refs/heads/main/security/signifyd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud
- Fraud Prevention
- Chargebacks
- Ecommerce
- Payments
- Risk
- Machine Learning
- Commerce Protection
- Account Protection
- Returns
---
