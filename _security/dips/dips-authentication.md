---
api_key_in:
- header
- query
api_specs:
- filename: dips-federation-service-openapi.yml
  format: yaml
  label: DIPS Federation Service
  slug: dips-federation-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dips/refs/heads/main/openapi/dips-federation-service-openapi.yml
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
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
