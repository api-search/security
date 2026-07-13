---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perpay.com
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.perpay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: api.perpay.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: help.perpay.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perpay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perpay, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perpay
provider_slug: perpay
slug: perpay-domain-security
source_filename: perpay-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perpay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.perpay.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\n- host: help.perpay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: perpay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perpay/refs/heads/main/security/perpay-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Fintech
- BNPL
- Buy Now Pay Later
- Credit Building
- Payroll Deduction
- Payments
- Consumer Finance
---
