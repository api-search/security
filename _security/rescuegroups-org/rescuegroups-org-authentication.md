---
api_key_in:
- header
api_specs:
- filename: rescuegroups-org-animals-api-openapi.yml
  format: yaml
  label: RescueGroups.org Animals API
  slug: rescuegroups-org-animals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-animals-api-openapi.yml
- filename: rescuegroups-org-authentication-api-openapi.yml
  format: yaml
  label: RescueGroups.org Authentication API
  slug: rescuegroups-org-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-authentication-api-openapi.yml
- filename: rescuegroups-org-breeds-api-openapi.yml
  format: yaml
  label: RescueGroups.org Breeds API
  slug: rescuegroups-org-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-breeds-api-openapi.yml
- filename: rescuegroups-org-colors-api-openapi.yml
  format: yaml
  label: RescueGroups.org Colors API
  slug: rescuegroups-org-colors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-colors-api-openapi.yml
- filename: rescuegroups-org-organizations-api-openapi.yml
  format: yaml
  label: RescueGroups.org Organizations API
  slug: rescuegroups-org-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-organizations-api-openapi.yml
- filename: rescuegroups-org-patterns-api-openapi.yml
  format: yaml
  label: RescueGroups.org Patterns API
  slug: rescuegroups-org-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-patterns-api-openapi.yml
- filename: rescuegroups-org-pet-lists-api-openapi.yml
  format: yaml
  label: RescueGroups.org Pet Lists API
  slug: rescuegroups-org-pet-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-pet-lists-api-openapi.yml
- filename: rescuegroups-org-species-api-openapi.yml
  format: yaml
  label: RescueGroups.org Species API
  slug: rescuegroups-org-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/openapi/rescuegroups-org-species-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rescuegroups Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: RescueGroups.org secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RescueGroups.org
provider_slug: rescuegroups-org
scheme_count: 2
schemes:
- description: API key authorization for public data access.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/rescuegroups-org-openapi.yml
  type: apiKey
- description: Bearer token for private/authenticated data access.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/rescuegroups-org-openapi.yml
  type: http
slug: rescuegroups-org-authentication
source_filename: rescuegroups-org-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rescuegroups-org-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authorization for public data access.\n  sources:\n  - openapi/rescuegroups-org-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for private/authenticated data access.\n  sources:\n  - openapi/rescuegroups-org-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rescuegroups-org/refs/heads/main/authentication/rescuegroups-org-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Animals
- Pet Adoption
- Rescue
- Animal Welfare
---
