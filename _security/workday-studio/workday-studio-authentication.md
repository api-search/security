---
api_key_in: []
api_specs:
- filename: workday-studio-integration-openapi.yml
  format: yaml
  label: Workday Studio Integration API
  slug: workday-studio-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-openapi.yml
- filename: workday-studio-web-services-openapi.yml
  format: yaml
  label: Workday Web Services API
  slug: workday-web-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-web-services-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Studio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Studio
provider_slug: workday-studio
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  sources:
  - openapi/workday-studio-integration-openapi.yml
  - openapi/workday-studio-web-services-openapi.yml
  type: oauth2
- description: WS-Security with X.509 certificates or username/password tokens for SOAP API authentication.
  name: WSSecurity
  scheme: basic
  sources:
  - openapi/workday-studio-web-services-openapi.yml
  type: http
slug: workday-studio-authentication
source_filename: workday-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-studio-integration-openapi.yml, openapi/workday-studio-web-services-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n    scopes: 2\n  sources:\n  - openapi/workday-studio-integration-openapi.yml\n  - openapi/workday-studio-web-services-openapi.yml\n- name: WSSecurity\n  type: http\n  scheme: basic\n  description: WS-Security with X.509 certificates or username/password tokens for SOAP API\n    authentication.\n  sources:\n  - openapi/workday-studio-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/authentication/workday-studio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud
- Development
- Enterprise
- Finance
- HR
- IDE
- Integration
---
