---
api_specs:
- filename: lean-authentication-api-openapi.yml
  format: yaml
  label: Lean Authentication API
  slug: lean-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-authentication-api-openapi.yml
- filename: lean-customers-api-openapi.yml
  format: yaml
  label: Lean Customers API
  slug: lean-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-customers-api-openapi.yml
- filename: lean-entities-api-openapi.yml
  format: yaml
  label: Lean Entities API
  slug: lean-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-entities-api-openapi.yml
- filename: lean-data-api-openapi.yml
  format: yaml
  label: Lean Data API
  slug: lean-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-data-api-openapi.yml
- filename: lean-insights-api-openapi.yml
  format: yaml
  label: Lean Insights API
  slug: lean-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-insights-api-openapi.yml
- filename: lean-banks-api-openapi.yml
  format: yaml
  label: Lean Banks API
  slug: lean-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-banks-api-openapi.yml
- filename: lean-verifications-api-openapi.yml
  format: yaml
  label: Lean Verifications API
  slug: lean-verifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-verifications-api-openapi.yml
- filename: lean-payments-api-openapi.yml
  format: yaml
  label: Lean Payments API
  slug: lean-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payments-api-openapi.yml
- filename: lean-payment-sources-api-openapi.yml
  format: yaml
  label: Lean Payment Sources API
  slug: lean-payment-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payment-sources-api-openapi.yml
- filename: lean-payouts-api-openapi.yml
  format: yaml
  label: Lean Payouts API
  slug: lean-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-payouts-api-openapi.yml
- filename: lean-refunds-api-openapi.yml
  format: yaml
  label: Lean Refunds API
  slug: lean-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/openapi/lean-refunds-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: leantech.me
  spf: true
hosts:
- cert_expires: Oct  2 13:05:30 2026 GMT
  host: www.leantech.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 18:04:07 2026 GMT
  host: docs.leantech.me
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 04:42:38 2026 GMT
  host: auth.leantech.me
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lean Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lean Technologies, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lean Technologies
provider_slug: lean-tech
slug: lean-tech-domain-security
source_filename: lean-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leantech.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:05:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.leantech.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 18:04:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.leantech.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 04:42:38 2026 GMT\n  hsts: null\ndomains:\n- domain: leantech.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-tech/refs/heads/main/security/lean-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Banking
- Open Finance
- MENA
- UAE
- Saudi Arabia
- Payments
- Pay by Bank
- A2A
- Account Information
- Payment Initiation
- Verifications
- Identity
- Fintech
---
