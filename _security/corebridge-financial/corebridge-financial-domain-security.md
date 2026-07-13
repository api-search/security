---
api_specs:
- filename: corebridgefinancial.yml
  format: yaml
  label: Corebridge Financial Website
  slug: website
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/corebridge-financial/refs/heads/main/openapi/corebridgefinancial.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: corebridgefinancial.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.corebridgefinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Corebridge Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Corebridge Financial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Corebridge Financial
provider_slug: corebridge-financial
slug: corebridge-financial-domain-security
source_filename: corebridge-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.corebridgefinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: corebridgefinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/corebridge-financial/refs/heads/main/security/corebridge-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AIG
- Annuities
- Financial Services
- Fortune 500
- Insurance
- K-12
- Life Insurance
- Retirement
- Variable Annuities
---
