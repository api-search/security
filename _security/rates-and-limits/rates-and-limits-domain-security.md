---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ratesandlimits.com
  spf: true
hosts:
- cert_expires: Nov 30 15:16:05 2026 GMT
  host: ratesandlimits.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Rates And Limits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rates and Limits, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rates and Limits
provider_slug: rates-and-limits
slug: rates-and-limits-domain-security
source_filename: rates-and-limits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ratesandlimits.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 15:16:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ratesandlimits.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rates-and-limits/refs/heads/main/security/rates-and-limits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Tax
- Payroll
- Benefits
- IRS
- minimum-wage
- Open Data
- Government
- Compliance
- Fintech
- Human Resources
- Reference Data
- JSON
- llms-txt
---
