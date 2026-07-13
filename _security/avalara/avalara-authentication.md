---
api_key_in: []
api_specs:
- filename: avalara-avatax-rest-openapi.yml
  format: yaml
  label: AvaTax APIs
  slug: avatax-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-rest-openapi.yml
- filename: avalara-communications-openapi.yml
  format: yaml
  label: Communications Tax API
  slug: communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-communications-openapi.yml
- filename: avalara-excise-openapi.yml
  format: yaml
  label: Excise Platform API
  slug: excise-tax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-excise-openapi.yml
- filename: avalara-item-classification-openapi.yml
  format: yaml
  label: Item Classification API
  slug: item-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-item-classification-openapi.yml
- filename: avalara-avatax-brazil-openapi.yml
  format: yaml
  label: AvaTax Brazil API
  slug: avatax-brazil-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-avatax-brazil-openapi.yml
- filename: avalara-vat-reporting-openapi.yml
  format: yaml
  label: VAT Reporting API
  slug: vat-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-vat-reporting-openapi.yml
- filename: avalara-mylodgetax-openapi.yml
  format: yaml
  label: MyLodgeTax API
  slug: mylodgetax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-mylodgetax-openapi.yml
- filename: avalara-certcapture-openapi.yml
  format: yaml
  label: CertCapture API
  slug: certcapture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-certcapture-openapi.yml
- filename: avalara-e-invoicing-openapi.yml
  format: yaml
  label: E-Invoicing REST API
  slug: e-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-e-invoicing-openapi.yml
- filename: avalara-activation-service-openapi.yml
  format: yaml
  label: Activation Service API
  slug: activation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-activation-service-openapi.yml
- filename: avalara-business-openapi.yml
  format: yaml
  label: Avalara Business API
  slug: business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-business-openapi.yml
- filename: avalara-portal-oauth-openapi.yml
  format: yaml
  label: Portal OAuth API
  slug: portal-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-portal-oauth-openapi.yml
- filename: avalara-shared-company-service-openapi.yml
  format: yaml
  label: Shared Company Service API
  slug: shared-company-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-shared-company-service-openapi.yml
- filename: avalara-hs-code-classification-openapi.yml
  format: yaml
  label: Automated Tariff Code Classification API
  slug: hs-code-classification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-hs-code-classification-openapi.yml
- filename: avalara-1099-w9-openapi.yml
  format: yaml
  label: 1099 & W-9 API
  slug: 1099-w9-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/openapi/avalara-1099-w9-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Avalara Authentication
name_suffix: Authentication
oauth_flows: []
overview: Avalara secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Avalara
provider_slug: avalara
scheme_count: 2
schemes:
- description: OAuth 2.0 bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/avalara-1099-w9-openapi.yml
  - openapi/avalara-activation-service-openapi.yml
  - openapi/avalara-avatax-brazil-openapi.yml
  - openapi/avalara-avatax-rest-openapi.yml
  - openapi/avalara-business-openapi.yml
  - openapi/avalara-e-invoicing-openapi.yml
  - openapi/avalara-excise-openapi.yml
  - openapi/avalara-hs-code-classification-openapi.yml
  - openapi/avalara-item-classification-openapi.yml
  - openapi/avalara-mylodgetax-openapi.yml
  - openapi/avalara-shared-company-service-openapi.yml
  - openapi/avalara-vat-reporting-openapi.yml
  type: http
- description: Use your AvaTax username/password or accountId/licenseKey as basic auth credentials
  name: basicAuth
  scheme: basic
  sources:
  - openapi/avalara-avatax-rest-openapi.yml
  - openapi/avalara-certcapture-openapi.yml
  - openapi/avalara-communications-openapi.yml
  - openapi/avatax-apis-openapi.yml
  type: http
slug: avalara-authentication
source_filename: avalara-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/avalara-1099-w9-openapi.yml, openapi/avalara-activation-service-openapi.yml,\n  openapi/avalara-avatax-brazil-openapi.yml, openapi/avalara-avatax-rest-openapi.yml, openapi/avalara-business-openapi.yml,\n  openapi/avalara-certcapture-openapi.yml, openapi/avalara-communications-openapi.yml, openapi/avalara-e-invoicing-openapi.yml,\n  openapi/avalara-excise-openapi.yml, openapi/avalara-hs-code-classification-openapi.yml, openapi/avalara-item-classification-openapi.yml,\n  openapi/avalara-mylodgetax-openapi.yml ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token\n  sources:\n  - openapi/avalara-1099-w9-openapi.yml\n  - openapi/avalara-activation-service-openapi.yml\n  - openapi/avalara-avatax-brazil-openapi.yml\n  - openapi/avalara-avatax-rest-openapi.yml\n  - openapi/avalara-business-openapi.yml\n  - openapi/avalara-e-invoicing-openapi.yml\n\
  \  - openapi/avalara-excise-openapi.yml\n  - openapi/avalara-hs-code-classification-openapi.yml\n  - openapi/avalara-item-classification-openapi.yml\n  - openapi/avalara-mylodgetax-openapi.yml\n  - openapi/avalara-shared-company-service-openapi.yml\n  - openapi/avalara-vat-reporting-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your AvaTax username/password or accountId/licenseKey as basic auth credentials\n  sources:\n  - openapi/avalara-avatax-rest-openapi.yml\n  - openapi/avalara-certcapture-openapi.yml\n  - openapi/avalara-communications-openapi.yml\n  - openapi/avatax-apis-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/authentication/avalara-authentication.yml
summary_line: http · 2 schemes
tags:
- Taxes
---
