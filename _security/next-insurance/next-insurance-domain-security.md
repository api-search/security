---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nextinsurance.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: www.nextinsurance.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Next Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ERGO NEXT Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ERGO NEXT Insurance
provider_slug: next-insurance
slug: next-insurance-domain-security
source_filename: next-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nextinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nextinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/next-insurance/refs/heads/main/security/next-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Property and Casualty
- Commercial Insurance
- Small Business
- SMB
- Embedded Insurance
- Workers Compensation
- General Liability
- Business Owners Policy
- Professional Liability
- Commercial Property
- Commercial Auto
- Underwriting
- Pay As You Go
- Munich Re
- ERGO
---
