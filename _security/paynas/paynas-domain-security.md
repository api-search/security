---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paynas.com
  spf: true
hosts:
- cert_expires: Oct 19 12:43:43 2026 GMT
  host: paynas.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Paynas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paynas, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paynas
provider_slug: paynas
slug: paynas-domain-security
source_filename: paynas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: paynas.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 19 12:43:43 2026 GMT\n  hsts: false\ndomains:\n- domain: paynas.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paynas/refs/heads/main/security/paynas-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- HR
- Payroll
- Human Resources
- Employee Benefits
- Fintech
- Payroll Cards
- Insurance
- Egypt
---
