---
api_key_in: []
api_specs:
- filename: zoho-creator-bulk-insert-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator Bulk Insert APIs API
  slug: zoho-creator-bulk-insert-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-bulk-insert-apis-api-openapi.yml
- filename: zoho-creator-bulk-read-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator Bulk Read APIs API
  slug: zoho-creator-bulk-read-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-bulk-read-apis-api-openapi.yml
- filename: zoho-creator-data-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator Data APIs API
  slug: zoho-creator-data-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-data-apis-api-openapi.yml
- filename: zoho-creator-file-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator File APIs API
  slug: zoho-creator-file-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-file-apis-api-openapi.yml
- filename: zoho-creator-meta-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator Meta APIs API
  slug: zoho-creator-meta-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-meta-apis-api-openapi.yml
- filename: zoho-creator-publish-apis-api-openapi.yml
  format: yaml
  label: Zoho Creator Publish APIs API
  slug: zoho-creator-publish-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/openapi/zoho-creator-publish-apis-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zoho Creator Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zoho Creator secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zoho Creator
provider_slug: zoho-creator
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.zoho.com/oauth/v2/auth?access_type=offline
    flow: authorizationCode
    scopes: 10
    tokenUrl: https://accounts.zoho.com/oauth/v2/token
  name: oauth2
  sources:
  - openapi/openapi.json
  type: oauth2
slug: zoho-creator-authentication
source_filename: zoho-creator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.zoho.com/oauth/v2/auth?access_type=offline\n    tokenUrl: https://accounts.zoho.com/oauth/v2/token\n    scopes: 10\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoho-creator/refs/heads/main/authentication/zoho-creator-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Low-Code
- Application Development
- No-Code
- Forms
- Records
- Workflows
- Database
- CRUD
- Business Applications
---
