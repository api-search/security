---
api_key_in: []
api_specs:
- filename: instapage-workspaces-api-openapi.yml
  format: yaml
  label: Instapage Workspaces API
  slug: instapage-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-workspaces-api-openapi.yml
- filename: instapage-analytics-api-openapi.yml
  format: yaml
  label: Instapage Analytics API
  slug: instapage-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-analytics-api-openapi.yml
- filename: instapage-assets-api-openapi.yml
  format: yaml
  label: Instapage Assets API
  slug: instapage-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-assets-api-openapi.yml
- filename: instapage-collections-api-openapi.yml
  format: yaml
  label: Instapage Collections API
  slug: instapage-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-collections-api-openapi.yml
- filename: instapage-domains-api-openapi.yml
  format: yaml
  label: Instapage Domains API
  slug: instapage-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-domains-api-openapi.yml
- filename: instapage-experiments-api-openapi.yml
  format: yaml
  label: Instapage Experiments API
  slug: instapage-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-experiments-api-openapi.yml
- filename: instapage-form-submissions-api-openapi.yml
  format: yaml
  label: Instapage Form Submissions API
  slug: instapage-form-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-form-submissions-api-openapi.yml
- filename: instapage-groups-api-openapi.yml
  format: yaml
  label: Instapage Groups API
  slug: instapage-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-groups-api-openapi.yml
- filename: instapage-pages-api-openapi.yml
  format: yaml
  label: Instapage Pages API
  slug: instapage-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-pages-api-openapi.yml
- filename: instapage-personalizations-api-openapi.yml
  format: yaml
  label: Instapage Personalizations API
  slug: instapage-personalizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-personalizations-api-openapi.yml
- filename: instapage-team-members-api-openapi.yml
  format: yaml
  label: Instapage Team Members API
  slug: instapage-team-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/openapi/instapage-team-members-api-openapi.yml
auth_types:
- http
description: Instapage authenticates every Public API request with a Personal API Token sent as an HTTP Bearer token in the Authorization header. There is no OAuth 2.0 authorization server, no scope surface and no client-credentials flow — the token is a long-lived personal credential generated from Instapage account settings.
kind: authentication
layout: security
method: searched
name: Instapage Authentication
name_suffix: Authentication
oauth_flows: []
overview: Instapage secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Instapage
provider_slug: instapage
scheme_count: 1
schemes:
- bearerFormat: Personal API Token
  docs: https://devdocs.instapage.com/
  header: Authorization
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/_original/instapage-openapi.yml
  type: http
  value_prefix: 'Bearer '
slug: instapage-authentication
source_filename: instapage-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://devdocs.instapage.com/\ndocs: https://devdocs.instapage.com/\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nmodel: personal-api-token\ndescription: >-\n  Instapage authenticates every Public API request with a Personal API Token sent as an HTTP Bearer\n  token in the Authorization header. There is no OAuth 2.0 authorization server, no scope surface and\n  no client-credentials flow — the token is a long-lived personal credential generated from Instapage\n  account settings.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: Personal API Token\n  header: Authorization\n  value_prefix: 'Bearer '\n  docs: https://devdocs.instapage.com/\n  sources:\n  - openapi/_original/instapage-openapi.yml\ntoken:\n  kind: personal-access-token\n  issued_from: Instapage account settings (dashboard)\n  issue_url: https://app.instapage.com/\n  rotation: manual (regenerate from account settings)\n\
  \  expiry: no published expiry; revoked tokens return 401\npermissions:\n  model: inherited\n  notes:\n  - A personal token inherits all permissions from its creator; access level may vary per workspace\n    depending on the creator's role in that workspace.\n  - Tokens cannot exceed the permissions granted to their creator.\n  - If the creator's permissions change (role update, removal), the token's access level is updated\n    automatically.\n  - Workspace-specific API limits also apply based on the workspace owner's plan.\n  - Expired or revoked tokens return 401 Unauthorized.\n  access_levels:\n  - viewer\n  - editor\n  - manager\n  - owner\n  quota_delegation:\n    field: inheritOwnerContextInPublicApi\n    description: >-\n      Workspace owners can set this flag on an individual team member. When true, that member's\n      public API requests count against the workspace owner's daily API quota instead of their own.\n    docs: https://devdocs.instapage.com/\noauth2: false\nmtls:\
  \ false\nopenid_connect: false\nx-evidence:\n- url: https://devdocs.instapage.com/\n  http_status: 200\n  section: Authorization / Limitations / Token Scope\n  fetched: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instapage/refs/heads/main/authentication/instapage-authentication.yml
summary_line: http · 1 scheme
tags:
- Landing Pages
- Conversion Optimization
- Marketing
- A/B Testing
- Post-Click Optimization
- Lead Generation
---
