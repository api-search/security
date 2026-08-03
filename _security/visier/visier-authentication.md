---
api_key_in:
- cookie
- header
api_specs:
- filename: visier-administration-apis-openapi.yaml
  format: yaml
  label: Visier Administration APIs
  slug: administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-administration-apis-openapi.yaml
- filename: visier-analytic-model-apis-openapi.yaml
  format: yaml
  label: Visier Analytic Model APIs
  slug: analytic-model
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-analytic-model-apis-openapi.yaml
- filename: visier-authentication-apis-openapi.yaml
  format: yaml
  label: Visier Authentication APIs
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-authentication-apis-openapi.yaml
- filename: visier-data-in-apis-openapi.yaml
  format: yaml
  label: Visier Data In APIs
  slug: data-in
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-in-apis-openapi.yaml
- filename: visier-data-out-apis-openapi.yaml
  format: yaml
  label: Visier Data Out APIs
  slug: data-out
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-data-out-apis-openapi.yaml
- filename: visier-webhooks-openapi.yaml
  format: yaml
  label: Visier Webhooks APIs
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-webhooks-openapi.yaml
- filename: visier-planning-openapi.yaml
  format: yaml
  label: Visier Planning Public APIs
  slug: planning
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-planning-openapi.yaml
- filename: visier-compensation-benchmarks-openapi.yaml
  format: yaml
  label: Visier Compensation Benchmarks API
  slug: compensation-benchmarks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-compensation-benchmarks-openapi.yaml
- filename: visier-skills-intelligence-engine-openapi.yaml
  format: yaml
  label: Visier Skills Intelligence Engine API
  slug: skills-intelligence-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/openapi/visier-skills-intelligence-engine-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Visier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
overview: Visier secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and password flow(s).
provider_name: Visier
provider_slug: visier
scheme_count: 5
schemes:
- in: cookie
  name: CookieAuth
  parameter: VisierASIDToken
  sources:
  - openapi/visier-administration-apis-openapi.yaml
  - openapi/visier-analytic-model-apis-openapi.yaml
  - openapi/visier-authentication-apis-openapi.yaml
  - openapi/visier-data-in-apis-openapi.yaml
  - openapi/visier-data-out-apis-openapi.yaml
  - openapi/visier-planning-openapi.yaml
  - openapi/visier-webhooks-openapi.yaml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: apikey
  sources:
  - openapi/visier-administration-apis-openapi.yaml
  - openapi/visier-analytic-model-apis-openapi.yaml
  - openapi/visier-authentication-apis-openapi.yaml
  - openapi/visier-compensation-benchmarks-openapi.yaml
  - openapi/visier-data-in-apis-openapi.yaml
  - openapi/visier-data-out-apis-openapi.yaml
  - openapi/visier-planning-openapi.yaml
  - openapi/visier-webhooks-openapi.yaml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/visier-administration-apis-openapi.yaml
  - openapi/visier-analytic-model-apis-openapi.yaml
  - openapi/visier-authentication-apis-openapi.yaml
  - openapi/visier-data-in-apis-openapi.yaml
  - openapi/visier-data-out-apis-openapi.yaml
  - openapi/visier-planning-openapi.yaml
  - openapi/visier-webhooks-openapi.yaml
  type: http
- flows:
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /v1/auth/oauth2/token
  - flow: password
    scopes: 2
    tokenUrl: /v1/auth/oauth2/token
  name: OAuth2Auth
  sources:
  - openapi/visier-administration-apis-openapi.yaml
  - openapi/visier-analytic-model-apis-openapi.yaml
  - openapi/visier-authentication-apis-openapi.yaml
  - openapi/visier-data-in-apis-openapi.yaml
  - openapi/visier-data-out-apis-openapi.yaml
  - openapi/visier-planning-openapi.yaml
  - openapi/visier-webhooks-openapi.yaml
  type: oauth2
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/visier-skills-intelligence-engine-openapi.yaml
  type: apiKey
slug: visier-authentication
source_filename: visier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/visier-administration-apis-openapi.yaml, openapi/visier-analytic-model-apis-openapi.yaml,\n  openapi/visier-authentication-apis-openapi.yaml, openapi/visier-compensation-benchmarks-openapi.yaml,\n  openapi/visier-data-in-apis-openapi.yaml, openapi/visier-data-out-apis-openapi.yaml, openapi/visier-planning-openapi.yaml,\n  openapi/visier-skills-intelligence-engine-openapi.yaml, openapi/visier-webhooks-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - password\nschemes:\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: VisierASIDToken\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n\
  \  - openapi/visier-webhooks-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-compensation-benchmarks-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n  - openapi/visier-webhooks-openapi.yaml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n  - openapi/visier-webhooks-openapi.yaml\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl:\
  \ /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/oauth2/token\n    scopes: 2\n  - flow: password\n    tokenUrl: /v1/auth/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/visier-administration-apis-openapi.yaml\n  - openapi/visier-analytic-model-apis-openapi.yaml\n  - openapi/visier-authentication-apis-openapi.yaml\n  - openapi/visier-data-in-apis-openapi.yaml\n  - openapi/visier-data-out-apis-openapi.yaml\n  - openapi/visier-planning-openapi.yaml\n  - openapi/visier-webhooks-openapi.yaml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/visier-skills-intelligence-engine-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/visier/refs/heads/main/authentication/visier-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- People Analytics
- Workforce Analytics
- Human Resources
- HR Technology
- Workforce Planning
- Analytics
- Business Intelligence
- Compensation
- Skills
- Artificial Intelligence
- Model Context Protocol
---
