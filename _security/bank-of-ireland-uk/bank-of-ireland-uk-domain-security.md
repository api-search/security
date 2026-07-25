---
api_specs:
- filename: bank-of-ireland-uk-open-data-openapi.json
  format: json
  label: Bank of Ireland (UK) Open Data API
  slug: bank-of-ireland-uk-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-open-data-openapi.json
- filename: bank-of-ireland-uk-account-info-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Account & Transaction Information API
  slug: bank-of-ireland-uk-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-account-info-openapi.yaml
- filename: bank-of-ireland-uk-payment-initiation-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Payment Initiation API
  slug: bank-of-ireland-uk-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-payment-initiation-openapi.yaml
- filename: bank-of-ireland-uk-confirmation-funds-openapi.yaml
  format: yaml
  label: Bank of Ireland (UK) Confirmation of Funds API
  slug: bank-of-ireland-uk-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/openapi/bank-of-ireland-uk-confirmation-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bankofirelanduk.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mulesoft.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.bankofirelanduk.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 23 23:59:59 2026 GMT
  host: eu1.anypoint.mulesoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: developer.bankofireland.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bank Of Ireland Uk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bank of Ireland (UK), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bank of Ireland (UK)
provider_slug: bank-of-ireland-uk
slug: bank-of-ireland-uk-domain-security
source_filename: bank-of-ireland-uk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bankofirelanduk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: eu1.anypoint.mulesoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.bankofireland.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bankofirelanduk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mulesoft.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bank-of-ireland-uk/refs/heads/main/security/bank-of-ireland-uk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- CMA9
- United Kingdom
- Payments
- Account Information
- Open Data
- FAPI
- Fintech
---
