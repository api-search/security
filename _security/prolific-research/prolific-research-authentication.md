---
api_key_in:
- header
api_specs:
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Studies API
  slug: prolific-research-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Submissions API
  slug: prolific-research-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Participant Groups API
  slug: prolific-research-participant-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Projects API
  slug: prolific-research-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Workspaces API
  slug: prolific-research-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Messages API
  slug: prolific-research-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Hooks (Webhooks) API
  slug: prolific-research-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Requirements & Filters API
  slug: prolific-research-requirements-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Bonuses API
  slug: prolific-research-bonuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
- filename: prolific-research-openapi.yml
  format: yaml
  label: Prolific Users API
  slug: prolific-research-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/openapi/prolific-research-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prolific Research Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prolific secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prolific
provider_slug: prolific-research
scheme_count: 1
schemes:
- description: API token supplied as "Token <your token>".
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/prolific-research-openapi.yml
  type: apiKey
slug: prolific-research-authentication
source_filename: prolific-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prolific-research-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API token supplied as \"Token <your token>\".\n  sources:\n  - openapi/prolific-research-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prolific-research/refs/heads/main/authentication/prolific-research-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Research
- Participant Recruitment
- Surveys
- Human Data
- Crowdsourcing
- Data Annotation
- AI Training
---
