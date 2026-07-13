---
api_key_in: []
api_specs:
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Account API
  slug: dotloop-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Profiles API
  slug: dotloop-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loops API
  slug: dotloop-loops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Details API
  slug: dotloop-loop-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop-It API
  slug: dotloop-loop-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Folders API
  slug: dotloop-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Documents API
  slug: dotloop-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Participants API
  slug: dotloop-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Tasks API
  slug: dotloop-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Activities API
  slug: dotloop-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Contacts API
  slug: dotloop-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Loop Templates API
  slug: dotloop-loop-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
- filename: dotloop-openapi.yml
  format: yaml
  label: dotloop Webhooks API
  slug: dotloop-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/openapi/dotloop-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Dotloop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: dotloop secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: dotloop
provider_slug: dotloop
scheme_count: 1
schemes:
- description: OAuth2 authorization code flow. Access tokens are short-lived (typically 12 hours) and passed as a Bearer token. Scopes include account:read, profile:read, profile:write, loop:read, loop:write, contact:read, contact:write, and template:read.
  flows:
  - authorizationUrl: https://auth.dotloop.com/oauth/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://auth.dotloop.com/oauth/token
  name: oauth2
  sources:
  - openapi/dotloop-openapi.yml
  type: oauth2
slug: dotloop-authentication
source_filename: dotloop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dotloop-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.dotloop.com/oauth/authorize\n    tokenUrl: https://auth.dotloop.com/oauth/token\n    scopes: 8\n  description: OAuth2 authorization code flow. Access tokens are short-lived (typically 12 hours)\n    and passed as a Bearer token. Scopes include account:read, profile:read, profile:write,\n    loop:read, loop:write, contact:read, contact:write, and template:read.\n  sources:\n  - openapi/dotloop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dotloop/refs/heads/main/authentication/dotloop-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Real Estate
- Transaction Management
- Loops
- Documents
- E-Signature
- Zillow Group
---
