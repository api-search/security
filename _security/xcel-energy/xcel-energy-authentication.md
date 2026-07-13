---
api_key_in: []
api_specs:
- filename: xcel-energy-green-button-api.yaml
  format: yaml
  label: Xcel Energy Green Button Connect My Data API
  slug: xcel-energy-green-button-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-green-button-api.yaml
- filename: xcel-energy-smart-meter-api.yaml
  format: yaml
  label: Xcel Energy Smart Meter IEEE 2030.5 API
  slug: xcel-energy-smart-meter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/openapi/xcel-energy-smart-meter-api.yaml
auth_types:
- http
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Xcel Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Xcel Energy secures its APIs with http, mutualTLS, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Xcel Energy
provider_slug: xcel-energy
scheme_count: 4
schemes:
- description: Customer-scoped access token issued via the OAuth 2.0 authorization-code grant.
  flows:
  - authorizationUrl: https://api.xcelenergy.com/DataCustodian/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token
  name: accessToken
  sources:
  - openapi/xcel-energy-green-button-api.yaml
  type: oauth2
- description: Application-scoped client access token used for management endpoints (Authorization list, Bulk, ServiceStatus).
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token
  name: clientAccessToken
  sources:
  - openapi/xcel-energy-green-button-api.yaml
  type: oauth2
- bearerFormat: Registration Access Token
  description: Token issued at application registration; used to read or update ApplicationInformation.
  name: registrationAccessToken
  scheme: bearer
  sources:
  - openapi/xcel-energy-green-button-api.yaml
  type: http
- description: IEEE 2030.5 requires mutual TLS authentication. Clients present a device certificate whose subject contains the LFDI/SFDI used to authorize access. Plain HTTP is not permitted.
  name: mtls
  sources:
  - openapi/xcel-energy-smart-meter-api.yaml
  type: mutualTLS
slug: xcel-energy-authentication
source_filename: xcel-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/xcel-energy-green-button-api.yaml, openapi/xcel-energy-smart-meter-api.yaml\nsummary:\n  types:\n  - http\n  - mutualTLS\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: accessToken\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.xcelenergy.com/DataCustodian/oauth/authorize\n    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token\n    scopes: 1\n  description: Customer-scoped access token issued via the OAuth 2.0 authorization-code grant.\n  sources:\n  - openapi/xcel-energy-green-button-api.yaml\n- name: clientAccessToken\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.xcelenergy.com/DataCustodian/oauth/token\n    scopes: 1\n  description: Application-scoped client access token used for management endpoints (Authorization\n    list, Bulk, ServiceStatus).\n  sources:\n  - openapi/xcel-energy-green-button-api.yaml\n\
  - name: registrationAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: Registration Access Token\n  description: Token issued at application registration; used to read or update ApplicationInformation.\n  sources:\n  - openapi/xcel-energy-green-button-api.yaml\n- name: mtls\n  type: mutualTLS\n  description: IEEE 2030.5 requires mutual TLS authentication. Clients present a device certificate\n    whose subject contains the LFDI/SFDI used to authorize access. Plain HTTP is not permitted.\n  sources:\n  - openapi/xcel-energy-smart-meter-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xcel-energy/refs/heads/main/authentication/xcel-energy-authentication.yml
summary_line: http/mutualTLS/oauth2 · 4 schemes
tags:
- Electric Utility
- Energy
- Energy Data
- Green Button
- Natural Gas
- Smart Grid
- Smart Meter
- Utility
- ESPI
- IEEE 2030.5
- Fortune 500
---
