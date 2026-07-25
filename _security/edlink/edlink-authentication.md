---
api_key_in: []
api_specs:
- filename: edlink-agents-api-openapi.yml
  format: yaml
  label: Edlink Agents API
  slug: edlink-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-agents-api-openapi.yml
- filename: edlink-classes-api-openapi.yml
  format: yaml
  label: Edlink Classes API
  slug: edlink-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-classes-api-openapi.yml
- filename: edlink-courses-api-openapi.yml
  format: yaml
  label: Edlink Courses API
  slug: edlink-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-courses-api-openapi.yml
- filename: edlink-districts-api-openapi.yml
  format: yaml
  label: Edlink Districts API
  slug: edlink-districts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-districts-api-openapi.yml
- filename: edlink-enrollments-api-openapi.yml
  format: yaml
  label: Edlink Enrollments API
  slug: edlink-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-enrollments-api-openapi.yml
- filename: edlink-events-api-openapi.yml
  format: yaml
  label: Edlink Events API
  slug: edlink-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-events-api-openapi.yml
- filename: edlink-graph-api-openapi.yml
  format: yaml
  label: Edlink Graph API
  slug: edlink-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-graph-api-openapi.yml
- filename: edlink-integrations-api-openapi.yml
  format: yaml
  label: Edlink Integrations API
  slug: edlink-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-integrations-api-openapi.yml
- filename: edlink-people-api-openapi.yml
  format: yaml
  label: Edlink People API
  slug: edlink-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-people-api-openapi.yml
- filename: edlink-schools-api-openapi.yml
  format: yaml
  label: Edlink Schools API
  slug: edlink-schools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-schools-api-openapi.yml
- filename: edlink-sections-api-openapi.yml
  format: yaml
  label: Edlink Sections API
  slug: edlink-sections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sections-api-openapi.yml
- filename: edlink-sso-api-openapi.yml
  format: yaml
  label: Edlink SSO API
  slug: edlink-sso-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-sso-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Edlink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Edlink secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Edlink
provider_slug: edlink
scheme_count: 1
schemes:
- description: Edlink Integration Access Token, User Access Token, or Meta API token passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/edlink-openapi.yml
  type: http
slug: edlink-authentication
source_filename: edlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/edlink-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Edlink Integration Access Token, User Access Token, or Meta API token passed\n    as a Bearer token.\n  sources:\n  - openapi/edlink-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/authentication/edlink-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- EdTech
- Rostering
- SIS
- LMS
- Integration
- Unified API
---
