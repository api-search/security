---
api_key_in:
- cookie
api_specs:
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Scripts API
  slug: windmill-dev-scripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Flows API
  slug: windmill-dev-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Apps API
  slug: windmill-dev-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Jobs API
  slug: windmill-dev-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Schedules API
  slug: windmill-dev-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Variables API
  slug: windmill-dev-variables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Resources API
  slug: windmill-dev-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workspaces API
  slug: windmill-dev-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Users API
  slug: windmill-dev-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Groups API
  slug: windmill-dev-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Folders API
  slug: windmill-dev-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Audit Logs API
  slug: windmill-dev-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Workers API
  slug: windmill-dev-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill Triggers API
  slug: windmill-dev-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
- filename: windmill-dev-openapi.yml
  format: yaml
  label: Windmill OIDC API
  slug: windmill-dev-oidc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/openapi/windmill-dev-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Windmill Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windmill secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Windmill
provider_slug: windmill-dev
scheme_count: 2
schemes:
- description: 'Bearer token created in the Windmill UI under account settings, passed as Authorization: Bearer YOUR_TOKEN.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/windmill-dev-openapi.yml
  type: http
- description: Session cookie set by the Windmill web UI after login.
  in: cookie
  name: cookieAuth
  parameter: token
  sources:
  - openapi/windmill-dev-openapi.yml
  type: apiKey
slug: windmill-dev-authentication
source_filename: windmill-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windmill-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token created in the Windmill UI under account settings, passed as Authorization:\n    Bearer YOUR_TOKEN.'\n  sources:\n  - openapi/windmill-dev-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: token\n  description: Session cookie set by the Windmill web UI after login.\n  sources:\n  - openapi/windmill-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windmill-dev/refs/heads/main/authentication/windmill-dev-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Platform
- Workflows
- Internal Tools
- Job Orchestration
- Cron
- Open Source
---
