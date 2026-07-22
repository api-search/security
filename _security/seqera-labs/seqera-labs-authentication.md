---
api_key_in: []
api_specs:
- filename: seqera-labs-platform-openapi.yml
  format: yaml
  label: Seqera Platform API
  slug: seqera-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seqera-labs/refs/heads/main/openapi/seqera-labs-platform-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Seqera Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seqera Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seqera Labs
provider_slug: seqera-labs
scheme_count: 1
schemes:
- bearerFormat: jwt
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/seqera-labs-platform-openapi.yml
  type: http
slug: seqera-labs-authentication
source_filename: seqera-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/seqera-labs-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  sources:\n  - openapi/seqera-labs-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seqera-labs/refs/heads/main/authentication/seqera-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Bioinformatics
- Workflow Orchestration
- Data Pipelines
- Scientific Computing
- Nextflow
- Cloud Compute
- Life Sciences
- Containers
- GA4GH
---
