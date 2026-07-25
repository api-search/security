---
api_specs:
- filename: clearbank-sterling-v4.json
  format: json
  label: ClearBank GBP Accounts API
  slug: clearbank-gbp-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sterling-v4.json
- filename: clearbank-fps-initiate-payment-v3.json
  format: json
  label: ClearBank Faster Payments API
  slug: clearbank-faster-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fps-initiate-payment-v3.json
- filename: clearbank-chaps-v6.json
  format: json
  label: ClearBank CHAPS API
  slug: clearbank-chaps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-chaps-v6.json
- filename: clearbank-mccy-accounts-v2.json
  format: json
  label: ClearBank Multi-Currency Accounts API
  slug: clearbank-multi-currency-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-accounts-v2.json
- filename: clearbank-mccy-payments-v1.json
  format: json
  label: ClearBank Multi-Currency Payments API
  slug: clearbank-multi-currency-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-mccy-payments-v1.json
- filename: clearbank-fx-orchestrator-rfq.json
  format: json
  label: ClearBank FX API
  slug: clearbank-fx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fx-orchestrator-rfq.json
- filename: clearbank-sepa-ct-v1.json
  format: json
  label: ClearBank SEPA Credit Transfer API
  slug: clearbank-sepa-credit-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sepa-ct-v1.json
- filename: clearbank-cop-outbound-v1.json
  format: json
  label: ClearBank Confirmation of Payee API
  slug: clearbank-confirmation-of-payee-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cop-outbound-v1.json
- filename: clearbank-know-your-customer-v1.json
  format: json
  label: ClearBank Customer Due Diligence (KYC) API
  slug: clearbank-customer-due-diligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-know-your-customer-v1.json
- filename: clearbank-cross-border-v4.json
  format: json
  label: ClearBank Cross-Border Sterling Payments API
  slug: clearbank-cross-border-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cross-border-v4.json
- filename: clearbank-customers_v2_retail.json
  format: json
  label: ClearBank Retail Embedded Banking Customers API
  slug: clearbank-retail-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customers_v2_retail.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: clear.bank
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: clearbank.co.uk
  spf: true
hosts:
- cert_expires: Oct  3 00:56:37 2026 GMT
  host: www.clear.bank
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 23:03:54 2026 GMT
  host: institution-api.clearbank.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClearBank, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: ClearBank
provider_slug: clearbank
slug: clearbank-domain-security
source_filename: clearbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clear.bank\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:56:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: institution-api.clearbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 23:03:54 2026 GMT\n  hsts: null\ndomains:\n- domain: clear.bank\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clearbank.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/security/clearbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Banking as a Service
- Embedded Banking
- Payments
- Clearing
- Faster Payments
- CHAPS
- Multi-Currency
- Foreign Exchange
- Open Banking
- United Kingdom
- Fintech
---
