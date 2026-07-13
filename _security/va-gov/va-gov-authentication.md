---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: VA Facilities API
  slug: va-facilities-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/facilities/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Forms API
  slug: va-forms-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/forms/v0/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Claims API
  slug: benefits-claims-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-claims/v2/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Intake API
  slug: benefits-intake-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-intake/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Documents API
  slug: benefits-documents-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-documents/v1/openapi.json
- filename: openapi.json
  format: json
  label: Benefits Reference Data API
  slug: benefits-reference-data-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/benefits-reference-data/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appeals Status API
  slug: appeals-status-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appeals-status/v1/openapi.json
- filename: openapi.json
  format: json
  label: Appealable Issues API
  slug: appealable-issues-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/appealable-issues/v0/openapi.json
- filename: openapi.json
  format: json
  label: Legacy Appeals API
  slug: legacy-appeals-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/legacy-appeals/v0/openapi.json
- filename: metadata
  format: yaml
  label: Patient Health API (FHIR)
  slug: patient-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: metadata
  format: yaml
  label: Clinical Health API (FHIR)
  slug: clinical-health-api
  spec_type: OpenAPI
  url: https://api.va.gov/services/fhir/v0/r4/metadata
- filename: openapi.json
  format: json
  label: Community Care Eligibility API
  slug: community-care-eligibility-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/community-care-eligibility/v0/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Verification API
  slug: veteran-verification-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-verification/v2/openapi.json
- filename: openapi.json
  format: json
  label: Veteran Confirmation API
  slug: veteran-confirmation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/veteran-confirmation/v1/openapi.json
- filename: openapi.json
  format: json
  label: Address Validation API
  slug: address-validation-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/address-validation/v3/openapi.json
- filename: openapi.json
  format: json
  label: Direct Deposit Management API
  slug: direct-deposit-management-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/direct-deposit-management/v1/openapi.json
- filename: openapi.json
  format: json
  label: VA Letter Generator API
  slug: va-letter-generator-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/va-letter-generator/v1/openapi.json
- filename: openapi.json
  format: json
  label: Loan Review API
  slug: loan-review-api
  spec_type: OpenAPI
  url: https://api.va.gov/internal/docs/loan-review/v1/openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Va Gov Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: VA Lighthouse secures its APIs with apiKey, http, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: VA Lighthouse
provider_slug: va-gov
scheme_count: 6
schemes:
- in: header
  name: apikey
  parameter: apikey
  sources:
  - openapi/va-gov-address-validation-v3-openapi.json
  - openapi/va-gov-appeals-status-v0-openapi.json
  - openapi/va-gov-benefits-intake-v1-openapi.json
  - openapi/va-gov-benefits-reference-data-v1-openapi.json
  - openapi/va-gov-facilities-v0-openapi.json
  - openapi/va-gov-facilities-v1-openapi.json
  - openapi/va-gov-forms-v0-openapi.json
  - openapi/va-gov-veteran-confirmation-v0-openapi.json
  type: apiKey
- description: 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code) and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token
  name: productionOauth
  sources:
  - openapi/va-gov-appealable-issues-v0-openapi.json
  - openapi/va-gov-appeals-status-v1-openapi.json
  - openapi/va-gov-legacy-appeals-v0-openapi.json
  - openapi/va-gov-veteran-verification-v2-openapi.json
  type: oauth2
- name: bearer_token
  scheme: bearer
  sources:
  - openapi/va-gov-benefits-claims-v1-openapi.json
  - openapi/va-gov-benefits-claims-v2-openapi.json
  - openapi/va-gov-veteran-verification-v0-openapi.json
  type: http
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)
  flows:
  - authorizationUrl: https://api.va.gov/oauth2/authorization
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.va.gov/oauth2/token
  name: productionOauth
  sources:
  - openapi/va-gov-benefits-claims-v1-openapi.json
  - openapi/va-gov-benefits-claims-v2-openapi.json
  - openapi/va-gov-community-care-eligibility-v0-openapi.json
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: https://api.va.gov/oauth2/exemplar/system/v1/token
  name: oauth2
  sources:
  - openapi/va-gov-benefits-documents-v1-openapi.json
  - openapi/va-gov-direct-deposit-management-v1-openapi.json
  - openapi/va-gov-loan-review-v1-openapi.json
  - openapi/va-gov-va-letter-generator-v1-openapi.json
  type: oauth2
- in: header
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/va-gov-veteran-confirmation-v1-openapi.json
  type: apiKey
slug: va-gov-authentication
source_filename: va-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/va-gov-address-validation-v3-openapi.json, openapi/va-gov-appealable-issues-v0-openapi.json,\n  openapi/va-gov-appeals-status-v0-openapi.json, openapi/va-gov-appeals-status-v1-openapi.json,\n  openapi/va-gov-benefits-claims-v1-openapi.json, openapi/va-gov-benefits-claims-v2-openapi.json,\n  openapi/va-gov-benefits-documents-v1-openapi.json, openapi/va-gov-benefits-intake-v1-openapi.json,\n  openapi/va-gov-benefits-reference-data-v1-openapi.json, openapi/va-gov-community-care-eligibility-v0-openapi.json,\n  openapi/va-gov-direct-deposit-management-v1-openapi.json, openapi/va-gov-facilities-v0-openapi.json\n  ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apikey\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/va-gov-address-validation-v3-openapi.json\n  - openapi/va-gov-appeals-status-v0-openapi.json\n\
  \  - openapi/va-gov-benefits-intake-v1-openapi.json\n  - openapi/va-gov-benefits-reference-data-v1-openapi.json\n  - openapi/va-gov-facilities-v0-openapi.json\n  - openapi/va-gov-facilities-v1-openapi.json\n  - openapi/va-gov-forms-v0-openapi.json\n  - openapi/va-gov-veteran-confirmation-v0-openapi.json\n- name: productionOauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/appeals/v1/authorization\n    tokenUrl: https://api.va.gov/oauth2/appeals/v1/token\n    scopes: 2\n  - flow: clientCredentials\n    tokenUrl: https://api.va.gov/oauth2/appeals/system/v1/token\n    scopes: 1\n  description: 'The authorization model for the Appealable Issues API uses OAuth 2.0/OpenID\n    Connect. The following models are supported: [Authorization Code Grant (ACG)](/explore/api/appealable-issues/authorization-code)\n    and [Client Credentials Grant (CCG)](/explore/api/appealable-issues/client-credentials).'\n  sources:\n  - openapi/va-gov-appealable-issues-v0-openapi.json\n\
  \  - openapi/va-gov-appeals-status-v1-openapi.json\n  - openapi/va-gov-legacy-appeals-v0-openapi.json\n  - openapi/va-gov-veteran-verification-v2-openapi.json\n- name: bearer_token\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/va-gov-benefits-claims-v1-openapi.json\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n  - openapi/va-gov-veteran-verification-v0-openapi.json\n- name: productionOauth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.va.gov/oauth2/authorization\n    tokenUrl: https://api.va.gov/oauth2/token\n    scopes: 2\n  description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://developer.va.gov/explore/api/benefits-claims/authorization-code)\n  sources:\n  - openapi/va-gov-benefits-claims-v1-openapi.json\n  - openapi/va-gov-benefits-claims-v2-openapi.json\n  - openapi/va-gov-community-care-eligibility-v0-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://api.va.gov/oauth2/exemplar/system/v1/token\n    scopes: 2\n  sources:\n  - openapi/va-gov-benefits-documents-v1-openapi.json\n  - openapi/va-gov-direct-deposit-management-v1-openapi.json\n  - openapi/va-gov-loan-review-v1-openapi.json\n  - openapi/va-gov-va-letter-generator-v1-openapi.json\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  sources:\n  - openapi/va-gov-veteran-confirmation-v1-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/va-gov/refs/heads/main/authentication/va-gov-authentication.yml
summary_line: apiKey/http/oauth2 · 6 schemes
tags:
- Government
- Veterans Affairs
- Veterans
- Healthcare
- Benefits
- FHIR
- Open Data
- Federal
---
