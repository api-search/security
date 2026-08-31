---
api_specs:
- filename: open-insurance-policy-api-openapi.yml
  format: yaml
  label: Open Policy API
  slug: open-insurance-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-insurance/refs/heads/main/openapi/open-insurance-policy-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beopen.com
  spf: true
hosts:
- cert_expires: Oct 21 03:39:59 2026 GMT
  host: www.beopen.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: insurance.beopen.com
  hsts: true
  hsts_max_age: 600
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 19:22:48 2026 GMT
  host: developers.beopen.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Open
provider_slug: open-insurance
slug: open-insurance-domain-security
source_filename: open-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.beopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 03:39:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: insurance.beopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 600\n- host: developers.beopen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 19:22:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: beopen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-insurance/refs/heads/main/security/open-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Australia
- Insurtech
- Embedded Insurance
- Property and Casualty
- Travel Insurance
- Underwriting
- Policy Administration
- White Label
- Quotes
---
