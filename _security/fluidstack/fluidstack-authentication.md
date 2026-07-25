---
api_key_in: []
api_specs:
- filename: fluidstack-clusters-api-openapi.yml
  format: yaml
  label: Fluidstack Clusters API
  slug: fluidstack-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-clusters-api-openapi.yml
- filename: fluidstack-instances-api-openapi.yml
  format: yaml
  label: Fluidstack Instances API
  slug: fluidstack-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-instances-api-openapi.yml
- filename: fluidstack-invitations-api-openapi.yml
  format: yaml
  label: Fluidstack Invitations API
  slug: fluidstack-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-invitations-api-openapi.yml
- filename: fluidstack-members-api-openapi.yml
  format: yaml
  label: Fluidstack Members API
  slug: fluidstack-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-members-api-openapi.yml
- filename: fluidstack-organizations-api-openapi.yml
  format: yaml
  label: Fluidstack Organizations API
  slug: fluidstack-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-organizations-api-openapi.yml
- filename: fluidstack-regions-api-openapi.yml
  format: yaml
  label: Fluidstack Regions API
  slug: fluidstack-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-regions-api-openapi.yml
- filename: fluidstack-user-api-openapi.yml
  format: yaml
  label: Fluidstack User API
  slug: fluidstack-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/openapi/fluidstack-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fluidstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fluidstack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fluidstack
provider_slug: fluidstack
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fluidstack-management-api-openapi.yml
  type: http
slug: fluidstack-authentication
source_filename: fluidstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fluidstack-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fluidstack-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluidstack/refs/heads/main/authentication/fluidstack-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- Artificial Intelligence
- GPU
- Cloud
- Compute
- Infrastructure
- Machine Learning
- Foundation Models
- Training
- Inference
- Kubernetes
- Slurm
- Bare Metal
- NVIDIA
- InfiniBand
- Data Centers
---
