---
anonymous_access: false
api_key_in: []
api_specs:
- filename: iproov-enrol-api-openapi.yml
  format: yaml
  label: iProov Enrol API
  slug: iproov-enrol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-enrol-api-openapi.yml
- filename: iproov-management-api-openapi.yml
  format: yaml
  label: iProov Management API
  slug: iproov-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-management-api-openapi.yml
- filename: iproov-user-api-openapi.yml
  format: yaml
  label: iProov User API
  slug: iproov-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-user-api-openapi.yml
- filename: iproov-verify-api-openapi.yml
  format: yaml
  label: iProov Verify API
  slug: iproov-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/iproov/openapi/iproov-verify-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Iproov Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: iProov secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: iProov
provider_slug: iproov
scheme_count: 2
schemes:
- description: OAuth2 is used for the Management and User APIs.
  flows:
  - flow: clientCredentials
    scopes: 2
    tokenUrl: /{api_key}/access_token
  name: oauth2
  sources:
  - openapi/iproov-openapi.yml
  type: oauth2
- description: These can now be obtained via the iPortal - OAuth Username and OAuth password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/iproov-openapi.yml
  type: http
slug: iproov-authentication
source_filename: iproov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/iproov-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /{api_key}/access_token\n    scopes: 2\n  description: OAuth2 is used for the Management and User APIs.\n  sources:\n  - openapi/iproov-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: These can now be obtained via the iPortal - OAuth Username and OAuth password.\n  sources:\n  - openapi/iproov-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/iproov/authentication/iproov-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Biometrics
- Identity Verification
- Authentication
- Liveness Detection
- Face Verification
- Fraud Prevention
- Deepfake Detection
---
