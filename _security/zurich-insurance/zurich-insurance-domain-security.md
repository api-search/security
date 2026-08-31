---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zurich.com
  spf: true
hosts:
- cert_expires: Sep  9 16:29:48 2026 GMT
  host: www.zurich.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 01:13:02 2026 GMT
  host: exchange.zurich.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zurich Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zurich Insurance, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zurich Insurance
provider_slug: zurich-insurance
slug: zurich-insurance-domain-security
source_filename: zurich-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zurich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 16:29:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: exchange.zurich.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: zurich.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zurich-insurance/refs/heads/main/security/zurich-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Financial
- Property & Casualty
- Open Insurance
- API Platform
---
