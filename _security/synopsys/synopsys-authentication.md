---
api_key_in:
- header
api_specs:
- filename: synopsys-polaris-openapi.yml
  format: yaml
  label: Synopsys Polaris API
  slug: polaris
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-polaris-openapi.yml
- filename: synopsys-cloud-openlink-openapi.yml
  format: yaml
  label: Synopsys Cloud OpenLink API
  slug: cloud-openlink
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/openapi/synopsys-cloud-openlink-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Synopsys Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Synopsys secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Synopsys
provider_slug: synopsys
scheme_count: 3
schemes:
- description: API key-based authentication
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/synopsys-cloud-openlink-openapi.yml
  type: apiKey
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.synopsys.com/oauth/token
  name: oauth2
  sources:
  - openapi/synopsys-cloud-openlink-openapi.yml
  type: oauth2
- description: Access token obtained from Polaris portal
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synopsys-polaris-openapi.yml
  type: http
slug: synopsys-authentication
source_filename: synopsys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synopsys-cloud-openlink-openapi.yml, openapi/synopsys-polaris-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key-based authentication\n  sources:\n  - openapi/synopsys-cloud-openlink-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.synopsys.com/oauth/token\n    scopes: 1\n  sources:\n  - openapi/synopsys-cloud-openlink-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Access token obtained from Polaris portal\n  sources:\n  - openapi/synopsys-polaris-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synopsys/refs/heads/main/authentication/synopsys-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Software Security
- Application Security Testing
- Static Analysis
- Software Composition Analysis
- EDA Tools
- Semiconductor Design
- Fortune 1000
---
