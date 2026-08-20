---
api_specs:
- filename: obie-opendata-swagger.json
  format: json
  label: Lloyds Banking Group Open Data API
  slug: open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/openapi/obie-opendata-swagger.json
- filename: obie-account-info-openapi.yaml
  format: yaml
  label: Lloyds Banking Group Account and Transaction Information API
  slug: account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/openapi/obie-account-info-openapi.yaml
- filename: obie-payment-initiation-openapi.yaml
  format: yaml
  label: Lloyds Banking Group Payment Initiation API
  slug: payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/openapi/obie-payment-initiation-openapi.yaml
- filename: obie-confirmation-funds-openapi.yaml
  format: yaml
  label: Lloyds Banking Group Confirmation of Funds API
  slug: confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/openapi/obie-confirmation-funds-openapi.yaml
- filename: obie-vrp-openapi.yaml
  format: yaml
  label: Lloyds Banking Group Variable Recurring Payments API
  slug: variable-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/openapi/obie-vrp-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lloydsbankinggroup.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lloydsbanking.com
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.lloydsbankinggroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 23:59:59 2026 GMT
  host: developer.lloydsbanking.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.lloydsbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lloyds Banking Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lloyds Banking Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Lloyds Banking Group
provider_slug: lloyds-banking-group
slug: lloyds-banking-group-domain-security
source_filename: lloyds-banking-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lloydsbankinggroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.lloydsbanking.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lloydsbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lloydsbankinggroup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: lloydsbanking.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lloyds-banking-group/refs/heads/main/security/lloyds-banking-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
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
---
