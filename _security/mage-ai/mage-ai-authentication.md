---
api_key_in:
- header
- query
api_specs:
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Triggers & Runs API
  slug: pipeline-triggers-runs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipelines API
  slug: pipelines
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Blocks API
  slug: blocks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
- filename: mage-ai-openapi.yml
  format: yaml
  label: Mage Pipeline Schedules API
  slug: schedules
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/openapi/mage-ai-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mage Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mage secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mage
provider_slug: mage-ai
scheme_count: 2
schemes:
- description: API key passed as the api_key query parameter or in the request body.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/mage-ai-openapi.yml
  type: apiKey
- description: Decoded OAuth token passed in the OAUTH-TOKEN header, or the raw token passed via the oauth_token cookie.
  in: header
  name: OAuthToken
  parameter: OAUTH-TOKEN
  sources:
  - openapi/mage-ai-openapi.yml
  type: apiKey
slug: mage-ai-authentication
source_filename: mage-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mage-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as the api_key query parameter or in the request body.\n  sources:\n  - openapi/mage-ai-openapi.yml\n- name: OAuthToken\n  type: apiKey\n  in: header\n  parameter: OAUTH-TOKEN\n  description: Decoded OAuth token passed in the OAUTH-TOKEN header, or the raw token passed\n    via the oauth_token cookie.\n  sources:\n  - openapi/mage-ai-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mage-ai/refs/heads/main/authentication/mage-ai-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Data Pipelines
- Orchestration
- ETL
- Data Engineering
- Open Source
---
