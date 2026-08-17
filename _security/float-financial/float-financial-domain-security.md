---
api_specs:
- filename: float-financial-openapi.yml
  format: yaml
  label: Float Public API
  slug: float-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/float-financial/refs/heads/main/openapi/float-financial-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: floatfinancial.com
  spf: true
hosts:
- cert_expires: Nov  4 23:14:48 2026 GMT
  host: floatfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 17:01:23 2026 GMT
  host: docs.floatfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: api.floatfinancial.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Float Financial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Float Financial, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Float Financial
provider_slug: float-financial
slug: float-financial-domain-security
source_filename: float-financial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: floatfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:14:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.floatfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:01:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.floatfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: floatfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/float-financial/refs/heads/main/security/float-financial-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- spend-management
- corporate-cards
- expense-management
- accounts-payable
- bill-pay
- reimbursements
- business-banking
- accounting-integration
- fintech
- canada
- payments
- erp-integration
---
