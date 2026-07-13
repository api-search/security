---
api_specs:
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Tax Calculations API
  slug: tax-calculations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Transactions API
  slug: transactions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
- filename: numeral-openapi.yml
  format: yaml
  label: Numeral Products & Tax Codes API
  slug: tax-codes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/openapi/numeral-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: numeral.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: numeralhq.com
  spf: true
hosts:
- cert_expires: Sep 25 22:16:57 2026 GMT
  host: www.numeral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 11:51:42 2026 GMT
  host: docs.numeral.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.numeralhq.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Numeral Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numeral, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Numeral
provider_slug: numeral
slug: numeral-domain-security
source_filename: numeral-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.numeral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:16:57 2026 GMT\n  hsts: false\n- host: docs.numeral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 11:51:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.numeralhq.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: numeral.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: numeralhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numeral/refs/heads/main/security/numeral-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sales Tax
- Tax Compliance
- Tax Calculation
- Ecommerce
- SaaS
---
