---
api_key_in:
- header
api_specs:
- filename: fiscalnote-bills-api-openapi.yml
  format: yaml
  label: FiscalNote Bills API
  slug: fiscalnote-bills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-bills-api-openapi.yml
- filename: fiscalnote-committees-api-openapi.yml
  format: yaml
  label: FiscalNote Committees API
  slug: fiscalnote-committees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-committees-api-openapi.yml
- filename: fiscalnote-issues-api-openapi.yml
  format: yaml
  label: FiscalNote Issues API
  slug: fiscalnote-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-issues-api-openapi.yml
- filename: fiscalnote-labels-api-openapi.yml
  format: yaml
  label: FiscalNote Labels API
  slug: fiscalnote-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-labels-api-openapi.yml
- filename: fiscalnote-legislation-api-openapi.yml
  format: yaml
  label: FiscalNote Legislation API
  slug: fiscalnote-legislation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-legislation-api-openapi.yml
- filename: fiscalnote-legislators-api-openapi.yml
  format: yaml
  label: FiscalNote Legislators API
  slug: fiscalnote-legislators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-legislators-api-openapi.yml
- filename: fiscalnote-officials-api-openapi.yml
  format: yaml
  label: FiscalNote Officials API
  slug: fiscalnote-officials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-officials-api-openapi.yml
- filename: fiscalnote-organizations-api-openapi.yml
  format: yaml
  label: FiscalNote Organizations API
  slug: fiscalnote-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-organizations-api-openapi.yml
- filename: fiscalnote-policy-intelligence-api-openapi.yml
  format: yaml
  label: FiscalNote Policy Intelligence API
  slug: fiscalnote-policy-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-policy-intelligence-api-openapi.yml
- filename: fiscalnote-presidential-transcripts-api-openapi.yml
  format: yaml
  label: FiscalNote Presidential Transcripts API
  slug: fiscalnote-presidential-transcripts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-presidential-transcripts-api-openapi.yml
- filename: fiscalnote-regulations-api-openapi.yml
  format: yaml
  label: FiscalNote Regulations API
  slug: fiscalnote-regulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-regulations-api-openapi.yml
- filename: fiscalnote-regulatory-documents-api-openapi.yml
  format: yaml
  label: FiscalNote Regulatory Documents API
  slug: fiscalnote-regulatory-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-regulatory-documents-api-openapi.yml
- filename: fiscalnote-stakeholders-api-openapi.yml
  format: yaml
  label: FiscalNote Stakeholders API
  slug: fiscalnote-stakeholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/openapi/fiscalnote-stakeholders-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fiscalnote Authentication
name_suffix: Authentication
oauth_flows: []
overview: FiscalNote secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FiscalNote
provider_slug: fiscalnote
scheme_count: 1
schemes:
- description: API key provided by FiscalNote. Include in the Authorization header of each request.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/fiscalnote-appdata-openapi.yml
  - openapi/fiscalnote-organization-openapi.yml
  - openapi/fiscalnote-people-openapi.yml
  - openapi/fiscalnote-policynote-openapi.yml
  type: apiKey
slug: fiscalnote-authentication
source_filename: fiscalnote-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fiscalnote-appdata-openapi.yml, openapi/fiscalnote-organization-openapi.yml,\n  openapi/fiscalnote-people-openapi.yml, openapi/fiscalnote-policynote-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key provided by FiscalNote. Include in the Authorization header of each request.\n  sources:\n  - openapi/fiscalnote-appdata-openapi.yml\n  - openapi/fiscalnote-organization-openapi.yml\n  - openapi/fiscalnote-people-openapi.yml\n  - openapi/fiscalnote-policynote-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiscalnote/refs/heads/main/authentication/fiscalnote-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Legislation
- Policy
- Political Intelligence
- Regulation
---
