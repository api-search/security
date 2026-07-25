---
api_specs:
- filename: teya-captures-api-openapi.yml
  format: yaml
  label: Teya Captures API
  slug: teya-captures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-captures-api-openapi.yml
- filename: teya-dcc-api-openapi.yml
  format: yaml
  label: Teya DCC API
  slug: teya-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-dcc-api-openapi.yml
- filename: teya-epos-registration-api-openapi.yml
  format: yaml
  label: Teya ePOS Registration API
  slug: teya-epos-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-epos-registration-api-openapi.yml
- filename: teya-hosted-checkout-api-openapi.yml
  format: yaml
  label: Teya Hosted Checkout API
  slug: teya-hosted-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-hosted-checkout-api-openapi.yml
- filename: teya-internal-api-openapi.yml
  format: yaml
  label: Teya '@internal' API
  slug: teya-internal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-internal-api-openapi.yml
- filename: teya-pay-at-table-api-openapi.yml
  format: yaml
  label: Teya Pay at Table API
  slug: teya-pay-at-table-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-pay-at-table-api-openapi.yml
- filename: teya-paybylink-api-openapi.yml
  format: yaml
  label: Teya PayByLink API
  slug: teya-paybylink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-paybylink-api-openapi.yml
- filename: teya-payment-requests-api-openapi.yml
  format: yaml
  label: Teya Payment Requests API
  slug: teya-payment-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-payment-requests-api-openapi.yml
- filename: teya-print-receipts-epos-api-openapi.yml
  format: yaml
  label: Teya Print Receipts (ePOS) API
  slug: teya-print-receipts-epos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-print-receipts-epos-api-openapi.yml
- filename: teya-public-api-openapi.yml
  format: yaml
  label: Teya '@public' API
  slug: teya-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-public-api-openapi.yml
- filename: teya-refunds-api-openapi.yml
  format: yaml
  label: Teya Refunds API
  slug: teya-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-refunds-api-openapi.yml
- filename: teya-reversals-api-openapi.yml
  format: yaml
  label: Teya Reversals API
  slug: teya-reversals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-reversals-api-openapi.yml
- filename: teya-stores-api-openapi.yml
  format: yaml
  label: Teya Stores API
  slug: teya-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-stores-api-openapi.yml
- filename: teya-terminals-api-openapi.yml
  format: yaml
  label: Teya Terminals API
  slug: teya-terminals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-terminals-api-openapi.yml
- filename: teya-tokens-api-openapi.yml
  format: yaml
  label: Teya Tokens API
  slug: teya-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-tokens-api-openapi.yml
- filename: teya-transactions-api-openapi.yml
  format: yaml
  label: Teya Transactions API
  slug: teya-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/openapi/teya-transactions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: saltpay.co
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teya.com
  spf: true
hosts:
- cert_expires: Oct  7 04:54:28 2026 GMT
  host: www.saltpay.co
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.teya.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: api.teya.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teya, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Teya
provider_slug: teya
slug: teya-domain-security
source_filename: teya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saltpay.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 04:54:28 2026 GMT\n  hsts: null\n- host: api.teya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\n- host: api.teya.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: saltpay.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: teya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teya/refs/heads/main/security/teya-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Payments
- Payment Processing
- Card Acquiring
- Online Payments
- Point of Sale
- E-commerce
- Fintech
- Merchant Services
- Europe
---
