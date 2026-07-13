---
api_specs:
- filename: wells-fargo-gateway-api-openapi.yml
  format: yaml
  label: Wells Fargo Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-gateway-api-openapi.yml
- filename: wells-fargo-account-transactions-api-openapi.yml
  format: yaml
  label: Wells Fargo Account Transactions API
  slug: account-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-account-transactions-api-openapi.yml
- filename: wells-fargo-ach-payments-api-openapi.yml
  format: yaml
  label: Wells Fargo ACH Payments API
  slug: ach-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/openapi/wells-fargo-ach-payments-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wellsfargo.com
  spf: true
hosts:
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: www.wellsfargo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: developer.wellsfargo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: api.wellsfargo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wells Fargo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wells-fargo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: wells-fargo
provider_slug: wells-fargo
slug: wells-fargo-domain-security
source_filename: wells-fargo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wellsfargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wellsfargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wellsfargo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wellsfargo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wells-fargo/refs/heads/main/security/wells-fargo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fortune 100
---
