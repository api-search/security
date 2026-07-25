---
api_key_in: []
api_specs:
- filename: rootly-alerts-api-openapi.yml
  format: yaml
  label: Rootly Alerts API
  slug: rootly-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-alerts-api-openapi.yml
- filename: rootly-escalation-policies-api-openapi.yml
  format: yaml
  label: Rootly Escalation Policies API
  slug: rootly-escalation-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-escalation-policies-api-openapi.yml
- filename: rootly-incidents-api-openapi.yml
  format: yaml
  label: Rootly Incidents API
  slug: rootly-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-incidents-api-openapi.yml
- filename: rootly-services-api-openapi.yml
  format: yaml
  label: Rootly Services API
  slug: rootly-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-services-api-openapi.yml
- filename: rootly-teams-api-openapi.yml
  format: yaml
  label: Rootly Teams API
  slug: rootly-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-teams-api-openapi.yml
- filename: rootly-users-api-openapi.yml
  format: yaml
  label: Rootly Users API
  slug: rootly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-users-api-openapi.yml
- filename: rootly-workflows-api-openapi.yml
  format: yaml
  label: Rootly Workflows API
  slug: rootly-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/openapi/rootly-workflows-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rootly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rootly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rootly
provider_slug: rootly
scheme_count: 1
schemes:
- description: 'Bearer token authentication. Pass your API token as `Authorization: Bearer [example key]`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rootly-openapi.yml
  type: http
slug: rootly-authentication
source_filename: rootly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rootly-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication. Pass your API token as `Authorization: Bearer [example key]`.'\n  sources:\n  - openapi/rootly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rootly/refs/heads/main/authentication/rootly-authentication.yml
summary_line: http · 1 scheme
tags:
- AIOps
- Incident Management
---
