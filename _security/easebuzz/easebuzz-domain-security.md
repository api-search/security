---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: easebuzz.in
  spf: true
hosts:
- cert_expires: Dec  2 13:13:28 2026 GMT
  host: easebuzz.in
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:56:39 2026 GMT
  host: docs.easebuzz.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 13:13:28 2026 GMT
  host: pay.easebuzz.in
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Easebuzz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Easebuzz, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Easebuzz
provider_slug: easebuzz
slug: easebuzz-domain-security
source_filename: easebuzz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: easebuzz.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 13:13:28 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\n- host: docs.easebuzz.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pay.easebuzz.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  2 13:13:28 2026 GMT\n  hsts: false\ndomains:\n- domain: easebuzz.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/easebuzz/refs/heads/main/security/easebuzz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Payment Gateway
- Payouts
- Banking
- India
- UPI
- Subscriptions
- SDK
---
