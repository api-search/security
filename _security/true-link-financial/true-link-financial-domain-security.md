---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truelinkfinancial.com
  spf: true
hosts:
- cert_expires: Oct  2 00:36:09 2026 GMT
  host: truelinkfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: True Link Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for True Link Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: True Link Financial
provider_slug: true-link-financial
slug: true-link-financial-domain-security
source_filename: true-link-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truelinkfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:36:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: truelinkfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/true-link-financial/refs/heads/main/security/true-link-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Prepaid Cards
- Wealth Management
- Payments
- Trust Management
- Elder Care
---
