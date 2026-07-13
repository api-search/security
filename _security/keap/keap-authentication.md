---
api_key_in: []
api_specs:
- filename: keap-openapi.yml
  format: yaml
  label: Keap REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/openapi/keap-openapi.yml
- filename: keap-resthooks-asyncapi.yml
  format: yaml
  label: Keap REST Hooks
  slug: rest-hooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/asyncapi/keap-resthooks-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Keap Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Keap secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Keap
provider_slug: keap
scheme_count: 1
schemes:
- description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/
  flows:
  - authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://api.infusionsoft.com/token
  name: oauth2
  sources:
  - openapi/keap-openapi.yml
  type: oauth2
slug: keap-authentication
source_filename: keap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keap-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.infusionsoft.com/app/oauth/authorize\n    tokenUrl: https://api.infusionsoft.com/token\n    scopes: 1\n  description: Keap uses OAuth 2.0 for authentication. See https://developer.infusionsoft.com/getting-started-oauth-keys/\n  sources:\n  - openapi/keap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keap/refs/heads/main/authentication/keap-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Marketing Automation
- Small Business
- E-Commerce
- Contacts
---
