---
anonymous_access: false
api_key_in: []
api_specs:
- filename: archbee-public-api-openapi.yml
  format: yaml
  label: Archbee Public API
  slug: archbee-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Archbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Archbee secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Archbee
provider_slug: archbee
scheme_count: 1
schemes:
- description: 'Requires the Authorization header in the form Authorization: Bearer {base64(docSpaceId~apiKey)} — the base64 encoding of the docSpaceId, a tilde, and the apiKey. A team key beginning abteam_ may be used instead to reach every space in the organization.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/archbee-public-api-openapi.yml
  type: http
slug: archbee-authentication
source_filename: archbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/archbee-public-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Requires the Authorization header in the form Authorization: Bearer {base64(docSpaceId~apiKey)}\n    — the base64 encoding of the docSpaceId, a tilde, and the apiKey. A team key beginning abteam_\n    may be used instead to reach every space in the organization.'\n  sources:\n  - openapi/archbee-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/authentication/archbee-authentication.yml
summary_line: http · 1 scheme
tags:
- API Documentation
- Documentation Platform
- Knowledge Base
- Technical Writing
- Developer Docs
- Developer Portal
- Docs as Code
- OpenAPI
- Model Context Protocol
- AI Agents
- Content Management
---
