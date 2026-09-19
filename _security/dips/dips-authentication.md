---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: dips-account-api-openapi.yml
  format: yaml
  label: DIPS Account API
  slug: dips-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-account-api-openapi.yml
- filename: dips-connect-api-openapi.yml
  format: yaml
  label: DIPS Connect API
  slug: dips-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-connect-api-openapi.yml
- filename: dips-consent-api-openapi.yml
  format: yaml
  label: DIPS Consent API
  slug: dips-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-consent-api-openapi.yml
- filename: dips-default-api-openapi.yml
  format: yaml
  label: DIPS * API
  slug: dips-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-default-api-openapi.yml
- filename: dips-home-api-openapi.yml
  format: yaml
  label: DIPS Home API
  slug: dips-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-home-api-openapi.yml
- filename: dips-login-api-openapi.yml
  format: yaml
  label: DIPS Login API
  slug: dips-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-login-api-openapi.yml
- filename: dips-status-api-openapi.yml
  format: yaml
  label: DIPS Status API
  slug: dips-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-status-api-openapi.yml
- filename: dips-well-known-api-openapi.yml
  format: yaml
  label: DIPS .well Known API
  slug: dips-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-well-known-api-openapi.yml
- filename: dips-user-role-api-openapi.yml
  format: yaml
  label: DIPS User Role API
  slug: dips-user-role-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-user-role-api-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: derived
name: Dips Authentication
name_suffix: Authentication
oauth_flows: []
overview: DIPS secures its APIs with apiKey and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DIPS
provider_slug: dips
scheme_count: 3
schemes:
- in: header
  name: apiKeyHeader
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/dips-federation-service-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: subscription-key
  sources:
  - openapi/dips-federation-service-openapi.yml
  type: apiKey
- name: openIdConnect
  openIdConnectUrl: https://api.dips.no/dips.oauth/.well-known/openid-configuration
  sources:
  - openapi/dips-federation-service-openapi.yml
  type: openIdConnect
slug: dips-authentication
source_filename: dips-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: derived\nsource: openapi/dips-federation-service-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/dips-federation-service-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: subscription-key\n  sources:\n  - openapi/dips-federation-service-openapi.yml\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.dips.no/dips.oauth/.well-known/openid-configuration\n  sources:\n  - openapi/dips-federation-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/authentication/dips-authentication.yml
summary_line: apiKey/openIdConnect · 3 schemes
tags:
- Company
- Healthcare
- Electronic Health Records
- Health IT
- FHIR
- openEHR
- Interoperability
- Identity
- OpenID Connect
- Norway
- Hospitals
- SMART on FHIR
---
