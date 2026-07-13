---
api_key_in: []
api_specs:
- filename: typeform-openapi.yml
  format: yaml
  label: Typeform Create API
  slug: create
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/openapi/typeform-openapi.yml
- filename: typeform-asyncapi.yml
  format: yaml
  label: Typeform Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/asyncapi/typeform-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Typeform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Typeform secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Typeform
provider_slug: typeform
scheme_count: 2
schemes:
- description: Personal access token or OAuth 2.0 access token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/typeform-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://api.typeform.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.typeform.com/oauth/token
  name: oauth2
  sources:
  - openapi/typeform-openapi.yml
  type: oauth2
slug: typeform-authentication
source_filename: typeform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/typeform-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Personal access token or OAuth 2.0 access token.\n  sources:\n  - openapi/typeform-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.typeform.com/oauth/authorize\n    tokenUrl: https://api.typeform.com/oauth/token\n    scopes: 6\n  sources:\n  - openapi/typeform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/authentication/typeform-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Forms
- Surveys
- Conversational
- Lead Capture
- SaaS
- Webhooks
- Embed
---
