---
api_key_in: []
api_specs:
- filename: formstack-asyncapi.yml
  format: yaml
  label: Formstack Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/openapi/formstack-asyncapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Formstack Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Formstack secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Formstack
provider_slug: formstack
scheme_count: 1
schemes:
- description: OAuth 2.0 authorization code flow.
  flows:
  - authorizationUrl: https://www.formstack.com/api/v2/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://www.formstack.com/api/v2/oauth2/token
  name: oauth2
  sources:
  - openapi/formstack-openapi.yml
  type: oauth2
slug: formstack-authentication
source_filename: formstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formstack-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.formstack.com/api/v2/oauth2/authorize\n    tokenUrl: https://www.formstack.com/api/v2/oauth2/token\n    scopes: 4\n  description: OAuth 2.0 authorization code flow.\n  sources:\n  - openapi/formstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formstack/refs/heads/main/authentication/formstack-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Forms
- Documents
- eSignature
- Workflow Automation
- No-Code
- OAuth2
---
