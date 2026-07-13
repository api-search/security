---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: Perforce Helix Core API
  slug: perforce-helix-core-api
  spec_type: OpenAPI
  url: https://api.perforce.com/helix-core/openapi.json
- filename: perforce-helix-swarm-openapi.yml
  format: yaml
  label: Perforce Helix Swarm API
  slug: perforce-helix-swarm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/perforce/refs/heads/main/openapi/perforce-helix-swarm-openapi.yml
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
