---
api_key_in: []
api_specs:
- filename: cch-tagetik-odata-openapi.yml
  format: yaml
  label: CCH Tagetik OData API
  slug: cch-tagetik-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tagetik/refs/heads/main/openapi/cch-tagetik-odata-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Tagetik Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CCH Tagetik secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CCH Tagetik
provider_slug: tagetik
scheme_count: 2
schemes:
- description: Basic authentication with CCH Tagetik username and password
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/cch-tagetik-odata-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{environment}/oauth2/token
  name: OAuth2ClientCredentials
  sources:
  - openapi/cch-tagetik-odata-openapi.yml
  type: oauth2
slug: tagetik-authentication
source_filename: tagetik-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cch-tagetik-odata-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with CCH Tagetik username and password\n  sources:\n  - openapi/cch-tagetik-odata-openapi.yml\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{environment}/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/cch-tagetik-odata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagetik/refs/heads/main/authentication/tagetik-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Analytics
- Budgeting
- Corporate Performance Management
- ESG
- Financial Close
- Financial Consolidation
- Financial Planning
- OData
- Reporting
---
