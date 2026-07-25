---
api_key_in: []
api_specs:
- filename: accelo-activities-api-openapi.yml
  format: yaml
  label: Accelo Activities API
  slug: accelo-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-activities-api-openapi.yml
- filename: accelo-companies-api-openapi.yml
  format: yaml
  label: Accelo Companies API
  slug: accelo-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-companies-api-openapi.yml
- filename: accelo-contacts-api-openapi.yml
  format: yaml
  label: Accelo Contacts API
  slug: accelo-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-contacts-api-openapi.yml
- filename: accelo-issues-api-openapi.yml
  format: yaml
  label: Accelo Issues API
  slug: accelo-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-issues-api-openapi.yml
- filename: accelo-jobs-api-openapi.yml
  format: yaml
  label: Accelo Jobs API
  slug: accelo-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-jobs-api-openapi.yml
- filename: accelo-oauth-api-openapi.yml
  format: yaml
  label: Accelo OAuth API
  slug: accelo-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-oauth-api-openapi.yml
- filename: accelo-tasks-api-openapi.yml
  format: yaml
  label: Accelo Tasks API
  slug: accelo-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/openapi/accelo-tasks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Accelo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Accelo secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Accelo
provider_slug: accelo
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token
  name: OAuth2
  sources:
  - openapi/accelo-openapi.yml
  type: oauth2
slug: accelo-authentication
source_filename: accelo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/accelo-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{deployment}.api.accelo.com/oauth2/v0/authorize\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\n    scopes: 0\n  - flow: clientCredentials\n    tokenUrl: https://{deployment}.api.accelo.com/oauth2/v0/token\n    scopes: 0\n  sources:\n  - openapi/accelo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accelo/refs/heads/main/authentication/accelo-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Professional Services Automation
- Project Management
- CRM
- Time Tracking
- Invoicing
- Service Operations
---
