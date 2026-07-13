---
api_key_in: []
api_specs:
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks LLM Interactions / Logging API
  slug: llm-interactions-logging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Applications / Versions API
  slug: applications-versions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Annotations API
  slug: annotations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
- filename: deepchecks-openapi.yml
  format: yaml
  label: Deepchecks Properties API
  slug: properties
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deepchecks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deepchecks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deepchecks
provider_slug: deepchecks
scheme_count: 1
schemes:
- description: Deepchecks API token, generated in the LLM Evaluation UI.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/deepchecks-openapi.yml
  type: http
slug: deepchecks-authentication
source_filename: deepchecks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deepchecks-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Deepchecks API token, generated in the LLM Evaluation UI.\n  sources:\n  - openapi/deepchecks-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/authentication/deepchecks-authentication.yml
summary_line: http · 1 scheme
tags:
- AI
- LLM
- Evaluation
- Testing
- Monitoring
---
