---
api_specs:
- filename: ameriprise.yml
  format: yaml
  label: Ameriprise Financial Website
  slug: website
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ameriprise-financial/refs/heads/main/openapi/ameriprise.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ameriprise.com
  spf: true
hosts:
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: www.ameriprise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ameriprise Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ameriprise Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ameriprise Financial
provider_slug: ameriprise-financial
slug: ameriprise-financial-domain-security
source_filename: ameriprise-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ameriprise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ameriprise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ameriprise-financial/refs/heads/main/security/ameriprise-financial-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial Planning
- Wealth Management
- Retirement
- Insurance
- Annuities
- Investment Management
- Financial Services
- Fortune 500
---
