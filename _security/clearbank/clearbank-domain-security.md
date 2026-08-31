---
api_specs:
- filename: clearbank-accounts-api-openapi.yml
  format: yaml
  label: ClearBank Accounts API
  slug: clearbank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-accounts-api-openapi.yml
- filename: clearbank-cop-api-openapi.yml
  format: yaml
  label: ClearBank Co P API
  slug: clearbank-cop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-cop-api-openapi.yml
- filename: clearbank-createfxquoteendpoint-api-openapi.yml
  format: yaml
  label: ClearBank Create Fx Quote Endpoint API
  slug: clearbank-createfxquoteendpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-createfxquoteendpoint-api-openapi.yml
- filename: clearbank-customer-api-openapi.yml
  format: yaml
  label: ClearBank Customer API
  slug: clearbank-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customer-api-openapi.yml
- filename: clearbank-customer-due-diligence-api-openapi.yml
  format: yaml
  label: ClearBank Customer Due Diligence API
  slug: clearbank-customer-due-diligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-customer-due-diligence-api-openapi.yml
- filename: clearbank-externalcrossbordercustomerpaymentsv4-api-openapi.yml
  format: yaml
  label: ClearBank External Cross Border Customer Payments V4 API
  slug: clearbank-externalcrossbordercustomerpaymentsv4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalcrossbordercustomerpaymentsv4-api-openapi.yml
- filename: clearbank-externalcustomerpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Customer Payments V6 API
  slug: clearbank-externalcustomerpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalcustomerpaymentsv6-api-openapi.yml
- filename: clearbank-externalinstitutionpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Institution Payments V6 API
  slug: clearbank-externalinstitutionpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalinstitutionpaymentsv6-api-openapi.yml
- filename: clearbank-externalreturnpaymentsv6-api-openapi.yml
  format: yaml
  label: ClearBank External Return Payments V6 API
  slug: clearbank-externalreturnpaymentsv6-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-externalreturnpaymentsv6-api-openapi.yml
- filename: clearbank-fpspayments-api-openapi.yml
  format: yaml
  label: ClearBank Fps Payments API
  slug: clearbank-fpspayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fpspayments-api-openapi.yml
- filename: clearbank-fx-orders-api-openapi.yml
  format: yaml
  label: ClearBank Fx Orders API
  slug: clearbank-fx-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-fx-orders-api-openapi.yml
- filename: clearbank-payments-api-openapi.yml
  format: yaml
  label: ClearBank Payments API
  slug: clearbank-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-payments-api-openapi.yml
- filename: clearbank-retail-api-openapi.yml
  format: yaml
  label: ClearBank Retail API
  slug: clearbank-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-retail-api-openapi.yml
- filename: clearbank-sct-payments-api-openapi.yml
  format: yaml
  label: ClearBank SCT Payments API
  slug: clearbank-sct-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-sct-payments-api-openapi.yml
- filename: clearbank-secondaryreferencedata-api-openapi.yml
  format: yaml
  label: ClearBank Secondary Reference Data API
  slug: clearbank-secondaryreferencedata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clearbank/refs/heads/main/openapi/clearbank-secondaryreferencedata-api-openapi.yml
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
- Financial-Services
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
