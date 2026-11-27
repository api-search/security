---
anonymous_access: false
api_key_in: []
api_specs:
- filename: artifacta-io-openapi.json
  format: json
  label: Artifacta API
  slug: artifacta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/artifacta-io/openapi/artifacta-io-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Artifacta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artifacta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Artifacta
provider_slug: artifacta-io
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/artifacta-io-openapi.json
  type: http
slug: artifacta-io-authentication
source_filename: artifacta-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/artifacta-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/artifacta-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/artifacta-io/authentication/artifacta-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Storage
- Artifact
- MCP
- Open Source
---
