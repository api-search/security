---
api_specs:
- filename: truv-openapi.yml
  format: yaml
  label: Truv Users API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Bridge Tokens API
  slug: bridge-tokens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Links API
  slug: links
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Employment Verification API
  slug: employment-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Income Verification API
  slug: income-verification
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Pay Statements API
  slug: pay-statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Direct Deposit Switch API
  slug: direct-deposit-switch
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Payroll & Shifts API
  slug: payroll-shifts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Insurance API
  slug: insurance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Identity & Banking API
  slug: identity-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
- filename: truv-openapi.yml
  format: yaml
  label: Truv Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/openapi/truv-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: truv.com
  spf: true
hosts:
- cert_expires: Jan 31 23:59:59 2027 GMT
  host: truv.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 10:21:35 2026 GMT
  host: docs.truv.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  9 23:59:59 2027 GMT
  host: prod.truv.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Truv Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truv, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truv
provider_slug: truv
slug: truv-domain-security
source_filename: truv-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 23:59:59 2027 GMT\n  hsts: false\n- host: docs.truv.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 10:21:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: prod.truv.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  9 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: truv.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truv/refs/heads/main/security/truv-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Income Verification
- Employment Verification
- Payroll
- Direct Deposit
- Consumer Permissioned Data
- Fintech
---
