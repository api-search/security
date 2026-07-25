---
api_key_in: []
api_specs:
- filename: outline-accessrequests-api-openapi.yml
  format: yaml
  label: Outline AccessRequests API
  slug: outline-accessrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-accessrequests-api-openapi.yml
- filename: outline-attachments-api-openapi.yml
  format: yaml
  label: Outline Attachments API
  slug: outline-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-attachments-api-openapi.yml
- filename: outline-auth-api-openapi.yml
  format: yaml
  label: Outline Auth API
  slug: outline-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-auth-api-openapi.yml
- filename: outline-collections-api-openapi.yml
  format: yaml
  label: Outline Collections API
  slug: outline-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-collections-api-openapi.yml
- filename: outline-comments-api-openapi.yml
  format: yaml
  label: Outline Comments API
  slug: outline-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-comments-api-openapi.yml
- filename: outline-dataattributes-api-openapi.yml
  format: yaml
  label: Outline DataAttributes API
  slug: outline-dataattributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-dataattributes-api-openapi.yml
- filename: outline-documents-api-openapi.yml
  format: yaml
  label: Outline Documents API
  slug: outline-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-documents-api-openapi.yml
- filename: outline-events-api-openapi.yml
  format: yaml
  label: Outline Events API
  slug: outline-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-events-api-openapi.yml
- filename: outline-fileoperations-api-openapi.yml
  format: yaml
  label: Outline FileOperations API
  slug: outline-fileoperations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-fileoperations-api-openapi.yml
- filename: outline-groups-api-openapi.yml
  format: yaml
  label: Outline Groups API
  slug: outline-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-groups-api-openapi.yml
- filename: outline-oauthauthentications-api-openapi.yml
  format: yaml
  label: Outline OAuthAuthentications API
  slug: outline-oauthauthentications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthauthentications-api-openapi.yml
- filename: outline-oauthclients-api-openapi.yml
  format: yaml
  label: Outline OAuthClients API
  slug: outline-oauthclients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-oauthclients-api-openapi.yml
- filename: outline-revisions-api-openapi.yml
  format: yaml
  label: Outline Revisions API
  slug: outline-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-revisions-api-openapi.yml
- filename: outline-shares-api-openapi.yml
  format: yaml
  label: Outline Shares API
  slug: outline-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-shares-api-openapi.yml
- filename: outline-stars-api-openapi.yml
  format: yaml
  label: Outline Stars API
  slug: outline-stars-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-stars-api-openapi.yml
- filename: outline-templates-api-openapi.yml
  format: yaml
  label: Outline Templates API
  slug: outline-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-templates-api-openapi.yml
- filename: outline-users-api-openapi.yml
  format: yaml
  label: Outline Users API
  slug: outline-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-users-api-openapi.yml
- filename: outline-views-api-openapi.yml
  format: yaml
  label: Outline Views API
  slug: outline-views-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/openapi/outline-views-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Outline Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Outline secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Outline
provider_slug: outline
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/outline-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.getoutline.com/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://app.getoutline.com/oauth/token
  name: OAuth2
  sources:
  - openapi/outline-openapi.yml
  type: oauth2
slug: outline-authentication
source_filename: outline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/outline-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/outline-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.getoutline.com/oauth/authorize\n    tokenUrl: https://app.getoutline.com/oauth/token\n    scopes: 2\n  sources:\n  - openapi/outline-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outline/refs/heads/main/authentication/outline-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Knowledge Base
- Wiki
- Documents
- Collaboration
- Open Source
- Team
---
