---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: functionalfi.com
  spf: true
hosts:
- cert_expires: Jan  9 22:15:56 2027 GMT
  host: www.functionalfi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Functional Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Functional Finance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Functional Finance
provider_slug: functional-finance
slug: functional-finance-domain-security
source_filename: functional-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.functionalfi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 22:15:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: functionalfi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/functional-finance/security/functional-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurance
- FinTech
- Payments
- Billing
- API
---
