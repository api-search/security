---
api_key_in: []
api_specs:
- filename: deepchecks-application-versions-api-openapi.yml
  format: yaml
  label: Deepchecks Application Versions API
  slug: deepchecks-application-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-application-versions-api-openapi.yml
- filename: deepchecks-applications-api-openapi.yml
  format: yaml
  label: Deepchecks Applications API
  slug: deepchecks-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-applications-api-openapi.yml
- filename: deepchecks-interactions-api-openapi.yml
  format: yaml
  label: Deepchecks Interactions API
  slug: deepchecks-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-interactions-api-openapi.yml
- filename: deepchecks-properties-api-openapi.yml
  format: yaml
  label: Deepchecks Properties API
  slug: deepchecks-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-properties-api-openapi.yml
- filename: deepchecks-spans-api-openapi.yml
  format: yaml
  label: Deepchecks Spans API
  slug: deepchecks-spans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-spans-api-openapi.yml
- filename: deepchecks-system-api-openapi.yml
  format: yaml
  label: Deepchecks System API
  slug: deepchecks-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deepchecks/refs/heads/main/openapi/deepchecks-system-api-openapi.yml
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
- Artificial Intelligence
- LLM
- Evaluation
- Testing
- Monitoring
---
