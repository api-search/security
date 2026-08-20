---
api_key_in: []
api_specs:
- filename: braintrust-data-acl-api-openapi.yml
  format: yaml
  label: Braintrust ACL API
  slug: braintrust-data-acl-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-acl-api-openapi.yml
- filename: braintrust-data-ai-proxy-api-openapi.yml
  format: yaml
  label: Braintrust AI Proxy API
  slug: braintrust-data-ai-proxy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-ai-proxy-api-openapi.yml
- filename: braintrust-data-credentials-api-openapi.yml
  format: yaml
  label: Braintrust Credentials API
  slug: braintrust-data-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-credentials-api-openapi.yml
- filename: braintrust-data-datasets-api-openapi.yml
  format: yaml
  label: Braintrust Datasets API
  slug: braintrust-data-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-datasets-api-openapi.yml
- filename: braintrust-data-evals-api-openapi.yml
  format: yaml
  label: Braintrust Evals API
  slug: braintrust-data-evals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-evals-api-openapi.yml
- filename: braintrust-data-experiments-api-openapi.yml
  format: yaml
  label: Braintrust Experiments API
  slug: braintrust-data-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-experiments-api-openapi.yml
- filename: braintrust-data-functions-api-openapi.yml
  format: yaml
  label: Braintrust Functions API
  slug: braintrust-data-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-functions-api-openapi.yml
- filename: braintrust-data-logs-api-openapi.yml
  format: yaml
  label: Braintrust Logs API
  slug: braintrust-data-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-logs-api-openapi.yml
- filename: braintrust-data-organization-api-openapi.yml
  format: yaml
  label: Braintrust Organization API
  slug: braintrust-data-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-organization-api-openapi.yml
- filename: braintrust-data-project-configuration-api-openapi.yml
  format: yaml
  label: Braintrust Project Configuration API
  slug: braintrust-data-project-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-project-configuration-api-openapi.yml
- filename: braintrust-data-projects-api-openapi.yml
  format: yaml
  label: Braintrust Projects API
  slug: braintrust-data-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-projects-api-openapi.yml
- filename: braintrust-data-prompts-api-openapi.yml
  format: yaml
  label: Braintrust Prompts API
  slug: braintrust-data-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/openapi/braintrust-data-prompts-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Braintrust Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Braintrust secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Braintrust
provider_slug: braintrust-data
scheme_count: 1
schemes:
- bearerFormat: API key or JWT
  description: 'Authenticate requests with your Braintrust API key in the Authorization header, e.g. `Authorization: Bearer $BRAINTRUST_API_KEY`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/braintrust-data-openapi.yml
  type: http
slug: braintrust-data-authentication
source_filename: braintrust-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/braintrust-data-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API key or JWT\n  description: 'Authenticate requests with your Braintrust API key in the Authorization header,\n    e.g. `Authorization: Bearer $BRAINTRUST_API_KEY`.'\n  sources:\n  - openapi/braintrust-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintrust-data/refs/heads/main/authentication/braintrust-data-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- LLM
- Evaluation
- Observability
- LLMOps
---
