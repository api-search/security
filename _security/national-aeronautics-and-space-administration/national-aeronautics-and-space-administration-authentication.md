---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: National Aeronautics And Space Administration Authentication
name_suffix: Authentication
oauth_flows: []
overview: The National Aeronautics and Space Administration secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The National Aeronautics and Space Administration
provider_slug: national-aeronautics-and-space-administration
scheme_count: 1
schemes:
- description: NASA API key (DEMO_KEY available for limited use).
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/national-aeronautics-and-space-administration-openapi.yml
  type: apiKey
slug: national-aeronautics-and-space-administration-authentication
source_filename: national-aeronautics-and-space-administration-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/national-aeronautics-and-space-administration-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: NASA API key (DEMO_KEY available for limited use).\n  sources:\n  - openapi/national-aeronautics-and-space-administration-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-aeronautics-and-space-administration/refs/heads/main/authentication/national-aeronautics-and-space-administration-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Science
- Space
- Imagery
- Earth Observation
---
