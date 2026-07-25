---
api_key_in: []
api_specs:
- filename: evrim-answers-api-openapi.yml
  format: yaml
  label: Evrim answers API
  slug: evrim-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-answers-api-openapi.yml
- filename: evrim-blank-api-openapi.yml
  format: yaml
  label: Evrim blank API
  slug: evrim-blank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-blank-api-openapi.yml
- filename: evrim-bulk-api-openapi.yml
  format: yaml
  label: Evrim bulk API
  slug: evrim-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-bulk-api-openapi.yml
- filename: evrim-collections-api-openapi.yml
  format: yaml
  label: Evrim collections API
  slug: evrim-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-collections-api-openapi.yml
- filename: evrim-compose-api-openapi.yml
  format: yaml
  label: Evrim compose API
  slug: evrim-compose-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-compose-api-openapi.yml
- filename: evrim-costs-api-openapi.yml
  format: yaml
  label: Evrim costs API
  slug: evrim-costs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-costs-api-openapi.yml
- filename: evrim-created-fields-api-openapi.yml
  format: yaml
  label: Evrim created-fields API
  slug: evrim-created-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-created-fields-api-openapi.yml
- filename: evrim-extract-api-openapi.yml
  format: yaml
  label: Evrim extract API
  slug: evrim-extract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-extract-api-openapi.yml
- filename: evrim-fields-api-openapi.yml
  format: yaml
  label: Evrim fields API
  slug: evrim-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-fields-api-openapi.yml
- filename: evrim-health-api-openapi.yml
  format: yaml
  label: Evrim health API
  slug: evrim-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-health-api-openapi.yml
- filename: evrim-prod-api-openapi.yml
  format: yaml
  label: Evrim prod API
  slug: evrim-prod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-prod-api-openapi.yml
- filename: evrim-profiles-api-openapi.yml
  format: yaml
  label: Evrim profiles API
  slug: evrim-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-profiles-api-openapi.yml
- filename: evrim-prompt-templates-api-openapi.yml
  format: yaml
  label: Evrim prompt-templates API
  slug: evrim-prompt-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-prompt-templates-api-openapi.yml
- filename: evrim-questions-api-openapi.yml
  format: yaml
  label: Evrim questions API
  slug: evrim-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-questions-api-openapi.yml
- filename: evrim-snapshots-api-openapi.yml
  format: yaml
  label: Evrim snapshots API
  slug: evrim-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-snapshots-api-openapi.yml
- filename: evrim-tags-api-openapi.yml
  format: yaml
  label: Evrim tags API
  slug: evrim-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-tags-api-openapi.yml
- filename: evrim-templates-api-openapi.yml
  format: yaml
  label: Evrim templates API
  slug: evrim-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-templates-api-openapi.yml
- filename: evrim-transform-api-openapi.yml
  format: yaml
  label: Evrim transform API
  slug: evrim-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/openapi/evrim-transform-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evrim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evrim secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Evrim
provider_slug: evrim
scheme_count: 1
schemes:
- applied_to_all_operations: true
  description: Django Knox API token presented as a Bearer credential in the Authorization header. Token supplied to the SDK via EVRIM_API_TOKEN.
  evidence:
  - https://github.com/evrimai/python-client/blob/HEAD/README.md
  name: knoxApiToken
  scheme: bearer
  sources:
  - openapi/evrim-openapi-original.yml
  type: http
slug: evrim-authentication
source_filename: evrim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/evrim-openapi-original.yml\ndocs: https://docs.evrim.ai\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nnotes: >-\n  Evrim authenticates every operation with a single Knox-issued API token\n  presented as an HTTP Bearer credential (Authorization: Bearer <token>). The\n  official Python SDK reads the token from the EVRIM_API_TOKEN environment\n  variable (or an `api_token` client keyword). All 91 operations apply the\n  knoxApiToken scheme; there is no OAuth2/OIDC and no API-key query or header\n  parameter.\nschemes:\n- name: knoxApiToken\n  type: http\n  scheme: bearer\n  description: >-\n    Django Knox API token presented as a Bearer credential in the Authorization\n    header. Token supplied to the SDK via EVRIM_API_TOKEN.\n  applied_to_all_operations: true\n  sources:\n  - openapi/evrim-openapi-original.yml\n  evidence:\n  - https://github.com/evrimai/python-client/blob/HEAD/README.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evrim/refs/heads/main/authentication/evrim-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Intelligence
- Signals
- Data Enrichment
- Profiles
- Entity Resolution
- Defense
- Financial Services
- Government
---
