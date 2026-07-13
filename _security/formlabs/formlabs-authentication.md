---
api_key_in: []
api_specs:
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Printers
  slug: formlabs-web-api-printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Prints
  slug: formlabs-web-api-prints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Consumables
  slug: formlabs-web-api-consumables
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Events
  slug: formlabs-web-api-events
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
- filename: formlabs-openapi.yml
  format: yaml
  label: Formlabs Web API (Dashboard) - Groups
  slug: formlabs-web-api-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/openapi/formlabs-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Formlabs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Formlabs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Formlabs
provider_slug: formlabs
scheme_count: 1
schemes:
- description: OAuth 2.0 Client Credentials flow. Exchange a client_id and client_secret at the token endpoint for a Bearer access token valid for 24 hours, scoped to developer-api. The Formlabs identity provider also supports OpenID Connect for interactive sign-in via PreForm / Local API.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.formlabs.com/developer/v1/o/token/
  name: OAuth2ClientCredentials
  sources:
  - openapi/formlabs-openapi.yml
  type: oauth2
slug: formlabs-authentication
source_filename: formlabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/formlabs-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.formlabs.com/developer/v1/o/token/\n    scopes: 1\n  description: OAuth 2.0 Client Credentials flow. Exchange a client_id and client_secret at\n    the token endpoint for a Bearer access token valid for 24 hours, scoped to developer-api.\n    The Formlabs identity provider also supports OpenID Connect for interactive sign-in via\n    PreForm / Local API.\n  sources:\n  - openapi/formlabs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formlabs/refs/heads/main/authentication/formlabs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- 3D Printing
- Additive Manufacturing
- SLA
- SLS
- Hardware
- Dashboard
---
