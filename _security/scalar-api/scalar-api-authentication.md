---
api_key_in: []
api_specs:
- filename: scalar-api-openapi.yml
  format: yaml
  label: Scalar Registry API
  slug: scalar-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalar-api/refs/heads/main/openapi/scalar-api-openapi.yml
- filename: galaxy
  format: yaml
  label: Scalar Galaxy API
  slug: scalar-galaxy-api
  spec_type: OpenAPI
  url: https://registry.scalar.com/@scalar/apis/galaxy?format=json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scalar Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalar secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalar
provider_slug: scalar-api
scheme_count: 1
schemes:
- description: Access to the Scalar hosted platform (Registry publish/manage, Docs deployment, SDK generation, Agent/MCP) is authenticated with a Scalar API key created in the Scalar dashboard (dashboard.scalar.com) and used by the Scalar CLI once you run `scalar auth login`. Scalar does not publish a fully documented public REST management API, so the exact header name and request shape are not officially specified - the CLI handles authentication on your behalf. The public registry read CDN (registry.scalar.com/@{namespace}/apis/{slug}) requires no auth for public documents. Authentication scheme is modeled (endpointsModeled).
  in: header
  name: scalarApiKey
  sources:
  - https://guides.scalar.com/scalar/scalar-registry/cli
  - https://guides.scalar.com/scalar/scalar-registry/getting-started
  type: apiKey
slug: scalar-api-authentication
source_filename: scalar-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: https://guides.scalar.com/scalar/scalar-registry/cli\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: scalarApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Access to the Scalar hosted platform (Registry publish/manage, Docs\n    deployment, SDK generation, Agent/MCP) is authenticated with a Scalar API\n    key created in the Scalar dashboard (dashboard.scalar.com) and used by the\n    Scalar CLI once you run `scalar auth login`. Scalar does not publish a fully\n    documented public REST management API, so the exact header name and request\n    shape are not officially specified - the CLI handles authentication on your\n    behalf. The public registry read CDN\n    (registry.scalar.com/@{namespace}/apis/{slug}) requires no auth for public\n    documents. Authentication scheme is modeled (endpointsModeled).\n  sources:\n  - https://guides.scalar.com/scalar/scalar-registry/cli\n  - https://guides.scalar.com/scalar/scalar-registry/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalar-api/refs/heads/main/authentication/scalar-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Documentation
- API Client
- Open Source
- Developer Tools
- API Reference
- OpenAPI
---
