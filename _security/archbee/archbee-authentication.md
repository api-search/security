---
anonymous_access: false
api_key_in: []
api_specs:
- filename: archbee-access-control-api-openapi.yml
  format: yaml
  label: Archbee Access Control API
  slug: archbee-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-access-control-api-openapi.yml
- filename: archbee-api-reference-api-openapi.yml
  format: yaml
  label: Archbee API Reference API
  slug: archbee-api-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-api-reference-api-openapi.yml
- filename: archbee-documents-api-openapi.yml
  format: yaml
  label: Archbee Documents API
  slug: archbee-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-documents-api-openapi.yml
- filename: archbee-file-manager-api-openapi.yml
  format: yaml
  label: Archbee File Manager API
  slug: archbee-file-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-file-manager-api-openapi.yml
- filename: archbee-members-api-openapi.yml
  format: yaml
  label: Archbee Members API
  slug: archbee-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-members-api-openapi.yml
- filename: archbee-organization-api-openapi.yml
  format: yaml
  label: Archbee Organization API
  slug: archbee-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-organization-api-openapi.yml
- filename: archbee-pages-api-openapi.yml
  format: yaml
  label: Archbee Pages API
  slug: archbee-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-pages-api-openapi.yml
- filename: archbee-space-groups-api-openapi.yml
  format: yaml
  label: Archbee Space Groups API
  slug: archbee-space-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-space-groups-api-openapi.yml
- filename: archbee-spaces-api-openapi.yml
  format: yaml
  label: Archbee Spaces API
  slug: archbee-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-spaces-api-openapi.yml
- filename: archbee-suggestions-api-openapi.yml
  format: yaml
  label: Archbee Suggestions API
  slug: archbee-suggestions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archbee/refs/heads/main/openapi/archbee-suggestions-api-openapi.yml
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
- MCP
- AI Agents
- Content Management
- Developer Tools
---
