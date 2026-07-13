---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payfit.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: payfit.io
  spf: true
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: payfit.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:43:41 2026 GMT
  host: developers.payfit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: partner-api.payfit.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Payfit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PayFit, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: PayFit
provider_slug: payfit
slug: payfit-domain-security
source_filename: payfit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payfit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: false\n- host: developers.payfit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: partner-api.payfit.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: payfit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: payfit.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payfit/refs/heads/main/security/payfit-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payroll
- Human Resources
- HR Tech
- Europe Payroll
- Time and Attendance
- Employee Management
---
