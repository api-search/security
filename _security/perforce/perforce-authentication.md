---
api_key_in: []
api_specs:
- filename: perforce-activity-api-openapi.yml
  format: yaml
  label: Perforce Activity API
  slug: perforce-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-activity-api-openapi.yml
- filename: perforce-changes-api-openapi.yml
  format: yaml
  label: Perforce Changes API
  slug: perforce-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-changes-api-openapi.yml
- filename: perforce-comments-api-openapi.yml
  format: yaml
  label: Perforce Comments API
  slug: perforce-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-comments-api-openapi.yml
- filename: perforce-projects-api-openapi.yml
  format: yaml
  label: Perforce Projects API
  slug: perforce-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-projects-api-openapi.yml
- filename: perforce-reviews-api-openapi.yml
  format: yaml
  label: Perforce Reviews API
  slug: perforce-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-reviews-api-openapi.yml
- filename: perforce-version-api-openapi.yml
  format: yaml
  label: Perforce Version API
  slug: perforce-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-version-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Perforce Authentication
name_suffix: Authentication
oauth_flows: []
overview: Perforce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Perforce
provider_slug: perforce
scheme_count: 1
schemes:
- description: HTTP Basic authentication using Perforce username and password or ticket. The password can be a standard Perforce password or a Swarm-generated API ticket.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/perforce-helix-swarm-openapi.yml
  type: http
slug: perforce-authentication
source_filename: perforce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/perforce-helix-swarm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using Perforce username and password or ticket. The\n    password can be a standard Perforce password or a Swarm-generated API ticket.\n  sources:\n  - openapi/perforce-helix-swarm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/authentication/perforce-authentication.yml
summary_line: http · 1 scheme
tags: []
---
