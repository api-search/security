---
api_key_in: []
api_specs:
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Users, Classes, Enrollments
  slug: graph-users-classes-enrollments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Schools, Districts
  slug: graph-schools-districts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Graph API - Courses, Sections
  slug: graph-courses-sections
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: SSO
  slug: sso
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Sources, Integrations
  slug: sources-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
- filename: edlink-openapi.yml
  format: yaml
  label: Events, Webhooks
  slug: events-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edlink/refs/heads/main/openapi/edlink-openapi.yml
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
