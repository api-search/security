---
api_key_in: []
api_specs:
- filename: paperspace-machines-api-openapi.yml
  format: yaml
  label: Paperspace Machines API
  slug: paperspace-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-machines-api-openapi.yml
- filename: paperspace-deployments-api-openapi.yml
  format: yaml
  label: Paperspace Deployments API
  slug: paperspace-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-deployments-api-openapi.yml
- filename: paperspace-projects-api-openapi.yml
  format: yaml
  label: Paperspace Projects API
  slug: paperspace-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-projects-api-openapi.yml
- filename: paperspace-datasets-api-openapi.yml
  format: yaml
  label: Paperspace Datasets API
  slug: paperspace-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-datasets-api-openapi.yml
- filename: paperspace-networking-api-openapi.yml
  format: yaml
  label: Paperspace Networking API
  slug: paperspace-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-networking-api-openapi.yml
- filename: paperspace-storage-api-openapi.yml
  format: yaml
  label: Paperspace Storage API
  slug: paperspace-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-storage-api-openapi.yml
- filename: paperspace-templates-api-openapi.yml
  format: yaml
  label: Paperspace Templates and Startup Scripts API
  slug: paperspace-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-templates-api-openapi.yml
- filename: paperspace-container-registries-api-openapi.yml
  format: yaml
  label: Paperspace Container Registries API
  slug: paperspace-container-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-container-registries-api-openapi.yml
- filename: paperspace-models-api-openapi.yml
  format: yaml
  label: Paperspace Models API
  slug: paperspace-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-models-api-openapi.yml
- filename: paperspace-team-auth-api-openapi.yml
  format: yaml
  label: Paperspace Team and Authentication API
  slug: paperspace-team-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/openapi/paperspace-team-auth-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Paperspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paperspace secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Paperspace
provider_slug: paperspace
scheme_count: 1
schemes:
- bearerFormat: api-key
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/paperspace-container-registries-api-openapi.yml
  - openapi/paperspace-datasets-api-openapi.yml
  - openapi/paperspace-deployments-api-openapi.yml
  - openapi/paperspace-machines-api-openapi.yml
  - openapi/paperspace-models-api-openapi.yml
  - openapi/paperspace-networking-api-openapi.yml
  - openapi/paperspace-projects-api-openapi.yml
  - openapi/paperspace-storage-api-openapi.yml
  - openapi/paperspace-team-auth-api-openapi.yml
  - openapi/paperspace-templates-api-openapi.yml
  type: http
slug: paperspace-authentication
source_filename: paperspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/paperspace-container-registries-api-openapi.yml, openapi/paperspace-datasets-api-openapi.yml,\n  openapi/paperspace-deployments-api-openapi.yml, openapi/paperspace-machines-api-openapi.yml,\n  openapi/paperspace-models-api-openapi.yml, openapi/paperspace-networking-api-openapi.yml,\n  openapi/paperspace-projects-api-openapi.yml, openapi/paperspace-storage-api-openapi.yml, openapi/paperspace-team-auth-api-openapi.yml,\n  openapi/paperspace-templates-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: api-key\n  sources:\n  - openapi/paperspace-container-registries-api-openapi.yml\n  - openapi/paperspace-datasets-api-openapi.yml\n  - openapi/paperspace-deployments-api-openapi.yml\n  - openapi/paperspace-machines-api-openapi.yml\n  - openapi/paperspace-models-api-openapi.yml\n  - openapi/paperspace-networking-api-openapi.yml\n  - openapi/paperspace-projects-api-openapi.yml\n\
  \  - openapi/paperspace-storage-api-openapi.yml\n  - openapi/paperspace-team-auth-api-openapi.yml\n  - openapi/paperspace-templates-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperspace/refs/heads/main/authentication/paperspace-authentication.yml
summary_line: http · 1 scheme
tags:
- GPU
- Cloud
- AI
- Machine Learning
- Deep Learning
- Compute
- DigitalOcean
- Containers
- Notebooks
- Gradient
---
