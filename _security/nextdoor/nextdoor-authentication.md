---
api_key_in: []
api_specs:
- filename: nextdoor-advertising-api-openapi.yml
  format: yaml
  label: Nextdoor Advertising API
  slug: nextdoor-advertising-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-advertising-api-openapi.yml
- filename: nextdoor-conversions-api-openapi.yml
  format: yaml
  label: Nextdoor Conversions API
  slug: nextdoor-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-conversions-api-openapi.yml
- filename: nextdoor-creatives-api-openapi.yml
  format: yaml
  label: Nextdoor Creatives API
  slug: nextdoor-creatives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-creatives-api-openapi.yml
- filename: nextdoor-posts-api-openapi.yml
  format: yaml
  label: Nextdoor Posts API
  slug: nextdoor-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-posts-api-openapi.yml
- filename: nextdoor-search-api-openapi.yml
  format: yaml
  label: Nextdoor Search API
  slug: nextdoor-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/openapi/nextdoor-search-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Nextdoor Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Nextdoor secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Nextdoor
provider_slug: nextdoor
scheme_count: 1
schemes:
- description: 'Nextdoor uses OAuth-based access tokens to authorize API

    requests. Refer to developer.nextdoor.com for token issuance

    and required scopes.'
  flows:
  - authorizationUrl: https://auth.nextdoor.com/v3/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.nextdoor.com/v3/token
  name: oauth2
  sources:
  - openapi/nextdoor-openapi.yml
  type: oauth2
slug: nextdoor-authentication
source_filename: nextdoor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/nextdoor-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.nextdoor.com/v3/authorize\n    tokenUrl: https://auth.nextdoor.com/v3/token\n    scopes: 0\n  description: |-\n    Nextdoor uses OAuth-based access tokens to authorize API\n    requests. Refer to developer.nextdoor.com for token issuance\n    and required scopes.\n  sources:\n  - openapi/nextdoor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nextdoor/refs/heads/main/authentication/nextdoor-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Social
- Local
- Advertising
- Community
- Sharing
---
