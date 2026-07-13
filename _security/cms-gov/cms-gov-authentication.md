---
api_key_in:
- query
api_specs:
- filename: cms-gov-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: blue-button-2-fhir-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-blue-button-2-openapi.yml
- filename: cms-gov-bcda-openapi.yml
  format: yaml
  label: CMS Beneficiary Claims Data API (BCDA)
  slug: beneficiary-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bcda-openapi.yml
- filename: cms-gov-ab2d-openapi.yml
  format: yaml
  label: CMS AB2D API
  slug: ab2d-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-ab2d-openapi.yml
- filename: cms-gov-dpc-openapi.yml
  format: yaml
  label: CMS Data at the Point of Care API (DPC)
  slug: data-at-point-of-care-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-dpc-openapi.yml
- filename: cms-gov-bfd-openapi.yml
  format: yaml
  label: CMS Beneficiary FHIR Data Server (BFD)
  slug: bfd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-bfd-openapi.yml
- filename: cms-gov-marketplace-openapi.yml
  format: yaml
  label: CMS Marketplace API
  slug: marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-marketplace-openapi.yml
- filename: cms-gov-open-data-openapi.yml
  format: yaml
  label: CMS Open Data API (data.cms.gov)
  slug: data-cms-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-open-data-openapi.yml
- filename: cms-gov-provider-data-openapi.yml
  format: yaml
  label: CMS Provider Data Catalog API
  slug: provider-data-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-provider-data-openapi.yml
- filename: cms-gov-qpp-openapi.yml
  format: yaml
  label: CMS Quality Payment Program API
  slug: quality-payment-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-qpp-openapi.yml
- filename: cms-gov-mcd-openapi.yml
  format: yaml
  label: CMS Medicare Coverage Database API
  slug: medicare-coverage-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/openapi/cms-gov-mcd-openapi.yml
auth_types:
- apiKey
- http
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cms Gov Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: CMS — Centers for Medicare & Medicaid Services secures its APIs with apiKey, http, mutualTLS, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: CMS — Centers for Medicare & Medicaid Services
provider_slug: cms-gov
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: AB2D uses SMART Backend Services with okta-issued JWT bearer tokens.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cms-gov-ab2d-openapi.yml
  - openapi/cms-gov-bcda-openapi.yml
  - openapi/cms-gov-dpc-openapi.yml
  - openapi/cms-gov-qpp-openapi.yml
  type: http
- description: BFD requires X.509 client certificates issued by the CMS PKI; access is restricted to peering applications.
  name: MutualTLS
  sources:
  - openapi/cms-gov-bfd-openapi.yml
  type: mutualTLS
- flows:
  - authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/
  name: OAuth2
  sources:
  - openapi/cms-gov-blue-button-2-openapi.yml
  type: oauth2
- in: query
  name: ApiKey
  parameter: apikey
  sources:
  - openapi/cms-gov-marketplace-openapi.yml
  type: apiKey
slug: cms-gov-authentication
source_filename: cms-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cms-gov-ab2d-openapi.yml, openapi/cms-gov-bcda-openapi.yml, openapi/cms-gov-bfd-openapi.yml,\n  openapi/cms-gov-blue-button-2-openapi.yml, openapi/cms-gov-dpc-openapi.yml, openapi/cms-gov-marketplace-openapi.yml,\n  openapi/cms-gov-qpp-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - mutualTLS\n  - oauth2\n  api_key_in:\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: AB2D uses SMART Backend Services with okta-issued JWT bearer tokens.\n  sources:\n  - openapi/cms-gov-ab2d-openapi.yml\n  - openapi/cms-gov-bcda-openapi.yml\n  - openapi/cms-gov-dpc-openapi.yml\n  - openapi/cms-gov-qpp-openapi.yml\n- name: MutualTLS\n  type: mutualTLS\n  description: BFD requires X.509 client certificates issued by the CMS PKI; access is restricted\n    to peering applications.\n  sources:\n  - openapi/cms-gov-bfd-openapi.yml\n\
  - name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.bluebutton.cms.gov/v2/o/authorize/\n    tokenUrl: https://api.bluebutton.cms.gov/v2/o/token/\n    scopes: 4\n  sources:\n  - openapi/cms-gov-blue-button-2-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/cms-gov-marketplace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-gov/refs/heads/main/authentication/cms-gov-authentication.yml
summary_line: apiKey/http/mutualTLS/oauth2 · 4 schemes
tags:
- Healthcare
- Medicare
- Medicaid
- FHIR
- Bulk Data
- Open Data
- Government
- Federal
- Claims
- Insurance
- ACA
- Marketplace
- Quality
---
