---
api_key_in: []
api_specs:
- filename: scope3-measurement-openapi.yml
  format: yaml
  label: Scope3 Carbon Calculator (Measurement) API
  slug: scope3-carbon-calculator-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-measurement-openapi.yml
- filename: scope3-ai-openapi-original.yml
  format: yaml
  label: Scope3 AI Impact Measurement API
  slug: scope3-ai-impact-measurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scope3/refs/heads/main/openapi/scope3-ai-openapi-original.yml
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
