---
api_key_in: []
api_specs:
- filename: spec.json
  format: json
  label: APIClarity API
  slug: apiclarity-api
  spec_type: OpenAPI
  url: https://github.com/openclarity/apiclarity/blob/master/api/server/restapi/spec.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Apiclarity Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIClarity secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIClarity
provider_slug: apiclarity
scheme_count: 1
schemes:
- description: APIClarity is typically deployed inside a Kubernetes cluster behind an ingress that enforces authentication. When exposed externally, deployments commonly require a bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/apiclarity-openapi.yml
  type: http
slug: apiclarity-authentication
source_filename: apiclarity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apiclarity-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: APIClarity is typically deployed inside a Kubernetes cluster behind an ingress\n    that enforces authentication. When exposed externally, deployments commonly require a bearer\n    token.\n  sources:\n  - openapi/apiclarity-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/authentication/apiclarity-authentication.yml
summary_line: http · 1 scheme
tags:
- API Observability
- API Security
- API Traffic Analysis
- Cisco
- Kubernetes
- Open Source
- OpenAPI Reconstruction
- OpenClarity
- Service Mesh
- Shadow APIs
---
