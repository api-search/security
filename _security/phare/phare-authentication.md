---
anonymous_access: false
api_key_in: []
api_specs:
- filename: phare-alert-rules-api-openapi.yml
  format: yaml
  label: Phare Alert Rules API
  slug: phare-alert-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-alert-rules-api-openapi.yml
- filename: phare-incidents-api-openapi.yml
  format: yaml
  label: Phare Incidents API
  slug: phare-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-incidents-api-openapi.yml
- filename: phare-integrations-api-openapi.yml
  format: yaml
  label: Phare Integrations API
  slug: phare-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-integrations-api-openapi.yml
- filename: phare-maintenance-windows-api-openapi.yml
  format: yaml
  label: Phare Maintenance Windows API
  slug: phare-maintenance-windows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-maintenance-windows-api-openapi.yml
- filename: phare-monitors-api-openapi.yml
  format: yaml
  label: Phare Monitors API
  slug: phare-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-monitors-api-openapi.yml
- filename: phare-platform-api-openapi.yml
  format: yaml
  label: Phare Platform API
  slug: phare-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-platform-api-openapi.yml
- filename: phare-projects-api-openapi.yml
  format: yaml
  label: Phare Projects API
  slug: phare-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-projects-api-openapi.yml
- filename: phare-reports-api-openapi.yml
  format: yaml
  label: Phare Reports API
  slug: phare-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-reports-api-openapi.yml
- filename: phare-status-pages-api-openapi.yml
  format: yaml
  label: Phare Status Pages API
  slug: phare-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-status-pages-api-openapi.yml
- filename: phare-users-api-openapi.yml
  format: yaml
  label: Phare Users API
  slug: phare-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/openapi/phare-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Phare Authentication
name_suffix: Authentication
oauth_flows: []
overview: Phare secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Phare
provider_slug: phare
scheme_count: 1
schemes:
- description: 'Use a user token to access authenticated routes. The token must be specified in the Authorization HTTP header with the following format ''Authorization: Bearer <token>''.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/phare-openapi.json
  type: http
slug: phare-authentication
source_filename: phare-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: derived\nsource: openapi/phare-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Use a user token to access authenticated routes. The token must be specified\n    in the Authorization HTTP header with the following format ''Authorization: Bearer <token>''.'\n  sources:\n  - openapi/phare-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phare/refs/heads/main/authentication/phare-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Monitoring
- Incident Management
- Analytics
- European
---
