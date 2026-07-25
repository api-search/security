---
api_key_in: []
api_specs:
- filename: bump-sh-branches-api-openapi.yml
  format: yaml
  label: Bump.sh Branches API
  slug: bump-sh-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-branches-api-openapi.yml
- filename: bump-sh-diffs-api-openapi.yml
  format: yaml
  label: Bump.sh Diffs API
  slug: bump-sh-diffs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-diffs-api-openapi.yml
- filename: bump-sh-hubs-api-openapi.yml
  format: yaml
  label: Bump.sh Hubs API
  slug: bump-sh-hubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-hubs-api-openapi.yml
- filename: bump-sh-mcp-servers-api-openapi.yml
  format: yaml
  label: Bump.sh MCP servers API
  slug: bump-sh-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-mcp-servers-api-openapi.yml
- filename: bump-sh-ping-api-openapi.yml
  format: yaml
  label: Bump.sh Ping API
  slug: bump-sh-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-ping-api-openapi.yml
- filename: bump-sh-previews-api-openapi.yml
  format: yaml
  label: Bump.sh Previews API
  slug: bump-sh-previews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-previews-api-openapi.yml
- filename: bump-sh-validations-api-openapi.yml
  format: yaml
  label: Bump.sh Validations API
  slug: bump-sh-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-validations-api-openapi.yml
- filename: bump-sh-versions-api-openapi.yml
  format: yaml
  label: Bump.sh Versions API
  slug: bump-sh-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/openapi/bump-sh-versions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bump Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bump.sh secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bump.sh
provider_slug: bump-sh
scheme_count: 2
schemes:
- name: Authorization token
  scheme: token
  sources:
  - openapi/bump-sh-openapi.yaml
  type: http
- name: Basic token
  scheme: basic
  sources:
  - openapi/bump-sh-openapi.yaml
  type: http
slug: bump-sh-authentication
source_filename: bump-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bump-sh-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: Authorization token\n  type: http\n  scheme: token\n  sources:\n  - openapi/bump-sh-openapi.yaml\n- name: Basic token\n  type: http\n  scheme: basic\n  sources:\n  - openapi/bump-sh-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bump-sh/refs/heads/main/authentication/bump-sh-authentication.yml
summary_line: http · 2 schemes
tags:
- API Changelog
- API Documentation
- API Hub
- API Governance
- Arazzo
- AsyncAPI
- CI/CD
- Flower
- MCP
- OpenAPI
- Workflows
---
