---
api_specs:
- filename: citi-authentication-api-1-openapi.yaml
  format: yaml
  label: Citi API Authentication Services
  slug: citi-api-authentication-services
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-authentication-api-1-openapi.yaml
- filename: citi-blocksandfilters-openapi.yaml
  format: yaml
  label: Citi Account Reporting APIs
  slug: citi-account-reporting-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-blocksandfilters-openapi.yaml
- filename: citi-digitalpaymentscollectionsv12-openapi.yaml
  format: yaml
  label: Citi Outgoing Payments APIs
  slug: citi-outgoing-payments-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-digitalpaymentscollectionsv12-openapi.yaml
- filename: citi-brazillocalmandate-openapi.yaml
  format: yaml
  label: Citi Payment Acceptance APIs
  slug: citi-payment-acceptance-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-brazillocalmandate-openapi.yaml
- filename: citi-marqueta-openapi.yaml
  format: yaml
  label: Citi Commercial Cards and Virtual Card Accounts APIs
  slug: citi-commercial-cards-and-virtual-card-accounts-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marqueta-openapi.yaml
- filename: citi-fx-authentication-api-openapi.yaml
  format: yaml
  label: CitiFX Gateway and Instant FX APIs
  slug: citifx-gateway-and-instant-fx-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-fx-authentication-api-openapi.yaml
- filename: citi-custody-billing-openapi.yaml
  format: yaml
  label: Citi Custody and Securities Services APIs
  slug: citi-custody-and-securities-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-custody-billing-openapi.yaml
- filename: citi-transfer-agency-accounts-openapi.yaml
  format: yaml
  label: Citi Funds Transfer Agency APIs
  slug: citi-funds-transfer-agency-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-transfer-agency-accounts-openapi.yaml
- filename: citi-ukraine-bank-data-sharing-api-openapi.yaml
  format: yaml
  label: Citi Open Banking APIs
  slug: citi-open-banking-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-ukraine-bank-data-sharing-api-openapi.yaml
- filename: citi-finance-undertaking-api-openapi.yaml
  format: yaml
  label: CitiConnect Trade Services APIs
  slug: citiconnect-trade-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-finance-undertaking-api-openapi.yaml
- filename: citi-marketplace-management-openapi.yaml
  format: yaml
  label: Citi Gateway Services API
  slug: citi-gateway-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-marketplace-management-openapi.yaml
- filename: citi-self-service-api-openapi.yaml
  format: yaml
  label: Citi Additional Payment Services APIs
  slug: citi-additional-payment-services-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/openapi/citi-self-service-api-openapi.yaml
description: ''
domains:
- caa:
  - 128 iodef "mailto:CAADNS@citi.com"
  - 128 issue "globalsign.com"
  - 128 issue "digicert.com"
  - 128 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: citi.com
  spf: true
hosts:
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: www.citi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 26 23:59:59 2027 GMT
  host: developer.citi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Citi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Citi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Citi
provider_slug: citi
slug: citi-domain-security
source_filename: citi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.citi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\n- host: developer.citi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 26 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: citi.com\n  dnssec: false\n  caa:\n  - 128 iodef \"mailto:CAADNS@citi.com\"\n  - 128 issue \"globalsign.com\"\n  - 128 issue \"digicert.com\"\n  - 128 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citi/refs/heads/main/security/citi-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Banking
- Financial-Services
- Open Banking
- Payments
- Treasury
- ISO 20022
- Commercial Cards
- Foreign Exchange
- Custody
- Trade Finance
- Corporate Banking
- API Gateway
---
