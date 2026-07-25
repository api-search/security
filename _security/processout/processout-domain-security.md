---
api_specs:
- filename: processout-balances-api-openapi.yml
  format: yaml
  label: ProcessOut Balances API
  slug: processout-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-balances-api-openapi.yml
- filename: processout-cards-api-openapi.yml
  format: yaml
  label: ProcessOut Cards API
  slug: processout-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-cards-api-openapi.yml
- filename: processout-customers-api-openapi.yml
  format: yaml
  label: ProcessOut Customers API
  slug: processout-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-customers-api-openapi.yml
- filename: processout-events-api-openapi.yml
  format: yaml
  label: ProcessOut Events API
  slug: processout-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-events-api-openapi.yml
- filename: processout-invoices-api-openapi.yml
  format: yaml
  label: ProcessOut Invoices API
  slug: processout-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-invoices-api-openapi.yml
- filename: processout-network-tokens-api-openapi.yml
  format: yaml
  label: ProcessOut Network Tokens API
  slug: processout-network-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-network-tokens-api-openapi.yml
- filename: processout-payouts-api-openapi.yml
  format: yaml
  label: ProcessOut Payouts API
  slug: processout-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-payouts-api-openapi.yml
- filename: processout-projects-api-openapi.yml
  format: yaml
  label: ProcessOut Projects API
  slug: processout-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-projects-api-openapi.yml
- filename: processout-transactions-api-openapi.yml
  format: yaml
  label: ProcessOut Transactions API
  slug: processout-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-transactions-api-openapi.yml
- filename: processout-uploads-api-openapi.yml
  format: yaml
  label: ProcessOut Uploads API
  slug: processout-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/openapi/processout-uploads-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: processout.com
  spf: true
hosts:
- cert_expires: Sep 11 05:23:52 2026 GMT
  host: processout.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.processout.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Processout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ProcessOut, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ProcessOut
provider_slug: processout
slug: processout-domain-security
source_filename: processout-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: processout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:23:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.processout.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: processout.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/processout/refs/heads/main/security/processout-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Payments
- Payment Orchestration
- Smart Routing
- Tokenization
- Checkout
- Reconciliation
- Fraud
- 3-D Secure
- Company
---
