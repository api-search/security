---
api_key_in: []
api_specs:
- filename: hyperscience-openapi.yml
  format: yaml
  label: Hyperscience REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/openapi/hyperscience-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Hyperscience Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hyperscience secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hyperscience
provider_slug: hyperscience
scheme_count: 1
schemes:
- description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{server}.{company}.com/oauth/token
  name: OAuth2
  sources:
  - openapi/hyperscience-openapi.yml
  type: oauth2
slug: hyperscience-authentication
source_filename: hyperscience-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hyperscience-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{server}.{company}.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 M2M with JWT bearer tokens issued by the tenant's local identity provider.\n  sources:\n  - openapi/hyperscience-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperscience/refs/heads/main/authentication/hyperscience-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- AI
- Document AI
- IDP
- Enterprise
- Automation
- GenAI
- FedRAMP
---
