---
api_key_in:
- header
api_specs:
- filename: mendix-apps-api-openapi.yml
  format: yaml
  label: Mendix Apps API
  slug: mendix-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-apps-api-openapi.yml
- filename: mendix-environments-api-openapi.yml
  format: yaml
  label: Mendix Environments API
  slug: mendix-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-environments-api-openapi.yml
- filename: mendix-logs-api-openapi.yml
  format: yaml
  label: Mendix Logs API
  slug: mendix-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-logs-api-openapi.yml
- filename: mendix-packages-api-openapi.yml
  format: yaml
  label: Mendix Packages API
  slug: mendix-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-packages-api-openapi.yml
- filename: mendix-tags-api-openapi.yml
  format: yaml
  label: Mendix Tags API
  slug: mendix-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/openapi/mendix-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mendix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mendix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mendix
provider_slug: mendix
scheme_count: 1
schemes:
- description: 'Mendix API key. Must be paired with a Mendix-Username header containing the

    login name of the user the key belongs to.'
  in: header
  name: mendixApiKey
  parameter: Mendix-ApiKey
  sources:
  - openapi/mendix-openapi.yml
  type: apiKey
slug: mendix-authentication
source_filename: mendix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mendix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: mendixApiKey\n  type: apiKey\n  in: header\n  parameter: Mendix-ApiKey\n  description: |-\n    Mendix API key. Must be paired with a Mendix-Username header containing the\n    login name of the user the key belongs to.\n  sources:\n  - openapi/mendix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mendix/refs/heads/main/authentication/mendix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Low-Code
- Application Development
- Enterprise Platform
- Application Lifecycle
- Deployment
- Governance
---
