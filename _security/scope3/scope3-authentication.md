---
api_key_in: []
api_specs:
- filename: scope3-ai-impact-measurement-api-openapi.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-impact-measurement-api-openapi.yml
- filename: scope3-benchmarks-api-openapi.yml
  format: yaml
  label: Scope3 Benchmarks API
  slug: scope3-benchmarks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-benchmarks-api-openapi.yml
- filename: scope3-creative-api-openapi.yml
  format: yaml
  label: Scope3 Creative API
  slug: scope3-creative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-creative-api-openapi.yml
- filename: scope3-data-api-openapi.yml
  format: yaml
  label: Scope3 Data API
  slug: scope3-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-data-api-openapi.yml
- filename: scope3-gpu-api-openapi.yml
  format: yaml
  label: Scope3 Gpu API
  slug: scope3-gpu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-gpu-api-openapi.yml
- filename: scope3-impact-api-openapi.yml
  format: yaml
  label: Scope3 Impact API
  slug: scope3-impact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-impact-api-openapi.yml
- filename: scope3-measure-api-openapi.yml
  format: yaml
  label: Scope3 Measure API
  slug: scope3-measure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measure-api-openapi.yml
- filename: scope3-model-api-openapi.yml
  format: yaml
  label: Scope3 Model API
  slug: scope3-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-model-api-openapi.yml
- filename: scope3-node-api-openapi.yml
  format: yaml
  label: Scope3 Node API
  slug: scope3-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-node-api-openapi.yml
- filename: scope3-reload-api-openapi.yml
  format: yaml
  label: Scope3 Reload API
  slug: scope3-reload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-reload-api-openapi.yml
- filename: scope3-saved-lists-api-openapi.yml
  format: yaml
  label: Scope3 Saved Lists API
  slug: scope3-saved-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-saved-lists-api-openapi.yml
- filename: scope3-segment-api-openapi.yml
  format: yaml
  label: Scope3 Segment API
  slug: scope3-segment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-segment-api-openapi.yml
- filename: scope3-signals-api-openapi.yml
  format: yaml
  label: Scope3 Signals API
  slug: scope3-signals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-signals-api-openapi.yml
- filename: scope3-status-api-openapi.yml
  format: yaml
  label: Scope3 Status API
  slug: scope3-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-status-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Scope3 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scope3 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scope3
provider_slug: scope3
scheme_count: 1
schemes:
- bearerFormat: JWT
  docs: https://docs.scope3.com/docs/access-authorization
  format: Bearer scope3_<accessClientId>_<accessClientSecret>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/scope3-ai-openapi-original.yml
  - openapi/scope3-measurement-openapi.yml
  type: http
slug: scope3-authentication
source_filename: scope3-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/scope3-ai-openapi-original.yml, openapi/scope3-measurement-openapi.yml\ndocs: https://docs.scope3.com/docs/access-authorization\nsummary:\n  types:\n  - http\n  token_format: \"scope3_<accessClientId>_<accessClientSecret>\"\n  header: Authorization\n  obtain: Contact your Scope3 representative for API access (dashboard key management at https://agentic.scope3.com for the Agentic Platform).\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  header: Authorization\n  format: \"Bearer scope3_<accessClientId>_<accessClientSecret>\"\n  docs: https://docs.scope3.com/docs/access-authorization\n  sources:\n  - openapi/scope3-ai-openapi-original.yml\n  - openapi/scope3-measurement-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/authentication/scope3-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Enterprise
- Advertising
- Carbon Emissions
- Sustainability
- AdTech
- Measurement
- Artificial Intelligence
- Agentic
---
