---
api_key_in: []
api_specs:
- filename: oxen-ai-api-openapi.yml
  format: yaml
  label: Oxen Ai API
  slug: oxen-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-ai-api-openapi.yml
- filename: oxen-branches-api-openapi.yml
  format: yaml
  label: Oxen Branches API
  slug: oxen-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-branches-api-openapi.yml
- filename: oxen-commits-api-openapi.yml
  format: yaml
  label: Oxen Commits API
  slug: oxen-commits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-commits-api-openapi.yml
- filename: oxen-compare-api-openapi.yml
  format: yaml
  label: Oxen Compare API
  slug: oxen-compare-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-compare-api-openapi.yml
- filename: oxen-data-frames-api-openapi.yml
  format: yaml
  label: Oxen Data Frames API
  slug: oxen-data-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-data-frames-api-openapi.yml
- filename: oxen-directories-api-openapi.yml
  format: yaml
  label: Oxen Directories API
  slug: oxen-directories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-directories-api-openapi.yml
- filename: oxen-evaluations-api-openapi.yml
  format: yaml
  label: Oxen evaluations API
  slug: oxen-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-evaluations-api-openapi.yml
- filename: oxen-export-api-openapi.yml
  format: yaml
  label: Oxen Export API
  slug: oxen-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-export-api-openapi.yml
- filename: oxen-files-api-openapi.yml
  format: yaml
  label: Oxen Files API
  slug: oxen-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-files-api-openapi.yml
- filename: oxen-fine-tunes-api-openapi.yml
  format: yaml
  label: Oxen fine_tunes API
  slug: oxen-fine-tunes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-fine-tunes-api-openapi.yml
- filename: oxen-health-api-openapi.yml
  format: yaml
  label: Oxen Health API
  slug: oxen-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-health-api-openapi.yml
- filename: oxen-import-api-openapi.yml
  format: yaml
  label: Oxen Import API
  slug: oxen-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-import-api-openapi.yml
- filename: oxen-merge-api-openapi.yml
  format: yaml
  label: Oxen Merge API
  slug: oxen-merge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-merge-api-openapi.yml
- filename: oxen-metadata-api-openapi.yml
  format: yaml
  label: Oxen Metadata API
  slug: oxen-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-metadata-api-openapi.yml
- filename: oxen-namespaces-api-openapi.yml
  format: yaml
  label: Oxen Namespaces API
  slug: oxen-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-namespaces-api-openapi.yml
- filename: oxen-repositories-api-openapi.yml
  format: yaml
  label: Oxen Repositories API
  slug: oxen-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-repositories-api-openapi.yml
- filename: oxen-version-files-api-openapi.yml
  format: yaml
  label: Oxen Version Files API
  slug: oxen-version-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-version-files-api-openapi.yml
- filename: oxen-workspace-files-api-openapi.yml
  format: yaml
  label: Oxen Workspace Files API
  slug: oxen-workspace-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-workspace-files-api-openapi.yml
- filename: oxen-workspaces-api-openapi.yml
  format: yaml
  label: Oxen Workspaces API
  slug: oxen-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/openapi/oxen-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Oxen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oxen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oxen
provider_slug: oxen
scheme_count: 1
schemes:
- description: 'Bearer API key. Header `Authorization: Bearer <OXEN_API_KEY>`. Same key across inference, fine-tuning, and version-control endpoints.'
  name: authorization
  scheme: bearer
  sources:
  - openapi/oxen-hub-api-openapi-original.json
  - openapi/oxen-server-openapi-original.json
  type: http
slug: oxen-authentication
source_filename: oxen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/oxen-hub-api-openapi-original.json, openapi/oxen-server-openapi-original.json\ndocs: https://docs.oxen.ai/getting-started/inference\nsummary:\n  types:\n  - http\n  model: >-\n    Oxen.ai authenticates every API request with a personal API key sent as an\n    HTTP Bearer token: `Authorization: Bearer $OXEN_API_KEY`. Keys are created in\n    account settings (https://www.oxen.ai/settings) and used identically by the\n    Hub AI/fine-tuning API, the data-version-control server API, the Python SDK\n    (oxenai), and the oxen CLI (`oxen config --auth hub.oxen.ai $TOKEN`). No OAuth\n    2.0 authorization-code / scope surface is published.\nschemes:\n- name: authorization\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer API key. Header `Authorization: Bearer <OXEN_API_KEY>`. Same key across\n    inference, fine-tuning, and version-control endpoints.\n  sources:\n  - openapi/oxen-hub-api-openapi-original.json\n\
  \  - openapi/oxen-server-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oxen/refs/heads/main/authentication/oxen-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data Version Control
- Machine Learning
- Artificial Intelligence
- Fine-Tuning
- Inference
- Datasets
- MLOps
- Large Language Models
- Model Deployment
- Developer Tools
- Version Control
---
