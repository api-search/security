---
api_key_in: []
api_specs:
- filename: looker-studio-assets-api-openapi.yml
  format: yaml
  label: Looker Studio Assets API
  slug: looker-studio-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-assets-api-openapi.yml
- filename: looker-studio-authentication-api-openapi.yml
  format: yaml
  label: Looker Studio Authentication API
  slug: looker-studio-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-authentication-api-openapi.yml
- filename: looker-studio-configuration-api-openapi.yml
  format: yaml
  label: Looker Studio Configuration API
  slug: looker-studio-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-configuration-api-openapi.yml
- filename: looker-studio-data-api-openapi.yml
  format: yaml
  label: Looker Studio Data API
  slug: looker-studio-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-data-api-openapi.yml
- filename: looker-studio-embed-api-openapi.yml
  format: yaml
  label: Looker Studio Embed API
  slug: looker-studio-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-embed-api-openapi.yml
- filename: looker-studio-manifest-api-openapi.yml
  format: yaml
  label: Looker Studio Manifest API
  slug: looker-studio-manifest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-manifest-api-openapi.yml
- filename: looker-studio-oembed-api-openapi.yml
  format: yaml
  label: Looker Studio oEmbed API
  slug: looker-studio-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-oembed-api-openapi.yml
- filename: looker-studio-permissions-api-openapi.yml
  format: yaml
  label: Looker Studio Permissions API
  slug: looker-studio-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-permissions-api-openapi.yml
- filename: looker-studio-reports-api-openapi.yml
  format: yaml
  label: Looker Studio Reports API
  slug: looker-studio-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-reports-api-openapi.yml
- filename: looker-studio-schema-api-openapi.yml
  format: yaml
  label: Looker Studio Schema API
  slug: looker-studio-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-schema-api-openapi.yml
- filename: looker-studio-visualization-api-openapi.yml
  format: yaml
  label: Looker Studio Visualization API
  slug: looker-studio-visualization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/openapi/looker-studio-visualization-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Looker Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Looker Studio secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Looker Studio
provider_slug: looker-studio
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication with domain-wide delegation. Requires Google Workspace or Cloud Identity organization.
  flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/looker-studio-api-openapi.yml
  type: oauth2
slug: looker-studio-authentication
source_filename: looker-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/looker-studio-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/v2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 3\n  description: OAuth 2.0 authentication with domain-wide delegation. Requires Google Workspace\n    or Cloud Identity organization.\n  sources:\n  - openapi/looker-studio-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/looker-studio/refs/heads/main/authentication/looker-studio-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Google
- Reports
---
