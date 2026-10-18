---
api_specs:
- filename: inscribe-bank-accounts-api-openapi.yml
  format: yaml
  label: Inscribe Bank Accounts API
  slug: inscribe-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-bank-accounts-api-openapi.yml
- filename: inscribe-collect-sessions-api-openapi.yml
  format: yaml
  label: Inscribe Collect Sessions API
  slug: inscribe-collect-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-collect-sessions-api-openapi.yml
- filename: inscribe-credit-insights-api-openapi.yml
  format: yaml
  label: Inscribe Credit Insights API
  slug: inscribe-credit-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-credit-insights-api-openapi.yml
- filename: inscribe-customers-api-openapi.yml
  format: yaml
  label: Inscribe Customers API
  slug: inscribe-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-customers-api-openapi.yml
- filename: inscribe-documents-api-openapi.yml
  format: yaml
  label: Inscribe Documents API
  slug: inscribe-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-documents-api-openapi.yml
- filename: inscribe-open-banking-api-openapi.yml
  format: yaml
  label: Inscribe Open Banking API
  slug: inscribe-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-open-banking-api-openapi.yml
- filename: inscribe-reachability-check-api-openapi.yml
  format: yaml
  label: Inscribe Reachability Check API
  slug: inscribe-reachability-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-reachability-check-api-openapi.yml
- filename: inscribe-transactions-api-openapi.yml
  format: yaml
  label: Inscribe Transactions API
  slug: inscribe-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-transactions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inscribe.ai
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.inscribe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 06:44:40 2026 GMT
  host: docs.inscribe.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: api.inscribe.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Inscribe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inscribe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inscribe
provider_slug: inscribe
slug: inscribe-domain-security
source_filename: inscribe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:44:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.inscribe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: inscribe.ai\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/security/inscribe-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fraud Prevention
- Document Verification
- Financial Services
- KYC
- KYB
- Bank Statements
- Paystubs
- Identity Verification
- Risk Management
- Fintech
- Artificial Intelligence
- Machine Learning
---
