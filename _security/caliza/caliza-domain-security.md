---
api_specs:
- filename: caliza-beneficiary-v1-api-openapi.yml
  format: yaml
  label: Caliza Beneficiary V1 API
  slug: caliza-beneficiary-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-beneficiary-v1-api-openapi.yml
- filename: caliza-integrator-capabilities-v1-api-openapi.yml
  format: yaml
  label: Caliza Integrator Capabilities V1 API
  slug: caliza-integrator-capabilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-integrator-capabilities-v1-api-openapi.yml
- filename: caliza-integrator-v1-api-openapi.yml
  format: yaml
  label: Caliza Integrator V1 API
  slug: caliza-integrator-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-integrator-v1-api-openapi.yml
- filename: caliza-kyc-kyb-v1-api-openapi.yml
  format: yaml
  label: Caliza KYC/KYB V1 API
  slug: caliza-kyc-kyb-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-kyc-kyb-v1-api-openapi.yml
- filename: caliza-payment-v1-api-openapi.yml
  format: yaml
  label: Caliza Payment V1 API
  slug: caliza-payment-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-payment-v1-api-openapi.yml
- filename: caliza-recipient-v1-api-openapi.yml
  format: yaml
  label: Caliza Recipient V1 API
  slug: caliza-recipient-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-recipient-v1-api-openapi.yml
- filename: caliza-related-person-api-openapi.yml
  format: yaml
  label: Caliza Related Person API
  slug: caliza-related-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-related-person-api-openapi.yml
- filename: caliza-terms-and-conditions-v1-api-openapi.yml
  format: yaml
  label: Caliza Terms and Conditions V1 API
  slug: caliza-terms-and-conditions-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-terms-and-conditions-v1-api-openapi.yml
- filename: caliza-transaction-v1-api-openapi.yml
  format: yaml
  label: Caliza Transaction V1 API
  slug: caliza-transaction-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-transaction-v1-api-openapi.yml
- filename: caliza-transaction-v1-sandbox-api-openapi.yml
  format: yaml
  label: Caliza Transaction V1 Sandbox API
  slug: caliza-transaction-v1-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-transaction-v1-sandbox-api-openapi.yml
- filename: caliza-travel-rule-v1-api-openapi.yml
  format: yaml
  label: Caliza Travel Rule V1 API
  slug: caliza-travel-rule-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-travel-rule-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caliza.com
  spf: true
hosts:
- cert_expires: Oct  2 06:56:36 2026 GMT
  host: www.caliza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 03:19:25 2026 GMT
  host: docs.caliza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: api.caliza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Caliza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caliza, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caliza
provider_slug: caliza
slug: caliza-domain-security
source_filename: caliza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caliza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 06:56:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.caliza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 03:19:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.caliza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: caliza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/security/caliza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Stablecoins
- Remittances
- Foreign Exchange
- Virtual Accounts
- Payouts
- KYC
- Latin America
---
