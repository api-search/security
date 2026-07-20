---
api_key_in:
- header
api_specs:
- filename: comet-opik-openapi-original.yml
  format: yaml
  label: Opik REST API
  slug: opik-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comet/refs/heads/main/openapi/comet-opik-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Comet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comet secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Comet
provider_slug: comet
scheme_count: 2
schemes:
- bearer_prefix: false
  description: Opik Cloud API key from your account settings, sent verbatim (no "Bearer " prefix).
  in: header
  name: OpikApiKey
  parameter: authorization
  type: apiKey
- description: Names the Comet/Opik workspace the request targets (required on Opik Cloud).
  in: header
  name: CometWorkspace
  parameter: Comet-Workspace
  type: apiKey
slug: comet-authentication
source_filename: comet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/comet-opik-openapi-original.yml\ndocs: https://www.comet.com/docs/opik/reference/rest-api/overview\nnote: >-\n  The Opik OpenAPI does not declare formal components.securitySchemes; auth is\n  documented in the spec info block and the REST API reference. Opik Cloud\n  authenticates with an API key passed in the \"authorization\" header (WITHOUT a\n  \"Bearer \" prefix) plus a \"Comet-Workspace\" header naming the workspace. The\n  open-source / self-hosted deployment (http://localhost:5173/api) requires no\n  auth headers. Enterprise SSO (OIDC/SAML/JWT) is available for the admin/web\n  surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: OpikApiKey\n  type: apiKey\n  in: header\n  parameter: authorization\n  bearer_prefix: false\n  description: Opik Cloud API key from your account settings, sent verbatim (no \"Bearer \" prefix).\n- name: CometWorkspace\n  type: apiKey\n\
  \  in: header\n  parameter: Comet-Workspace\n  description: Names the Comet/Opik workspace the request targets (required on Opik Cloud).\nenterprise_sso:\n  docs: https://www.comet.com/docs/opik/administration/authentication/overview\n  methods:\n  - oidc\n  - saml\n  - jwt\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comet/refs/heads/main/authentication/comet-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ai Enterprise Software
- LLM Observability
- LLMOps
- MLOps
- Evaluation
- Experiment Tracking
- Model Monitoring
- Prompt Management
- Agents
- Open Source
---
