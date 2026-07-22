---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alogent.com
  spf: true
hosts:
- cert_expires: Sep 20 15:37:28 2026 GMT
  host: www.alogent.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alogent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alogent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alogent
provider_slug: alogent
slug: alogent-domain-security
source_filename: alogent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alogent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:37:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: alogent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alogent/refs/heads/main/security/alogent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Banking
- Financial Services
- Fintech
- Payments
- Check Processing
- Deposit Automation
- Fraud Detection
- Content Management
- Loan Management
---
