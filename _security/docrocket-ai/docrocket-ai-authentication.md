---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docrocket-ai-brand-from-url-api-openapi.yml
  format: yaml
  label: docrocket-ai Brand From Url API
  slug: docrocket-ai-brand-from-url-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-brand-from-url-api-openapi.yml
- filename: docrocket-ai-generate-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Generate Document API
  slug: docrocket-ai-generate-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-generate-document-api-openapi.yml
- filename: docrocket-ai-get-document-api-openapi.yml
  format: yaml
  label: docrocket-ai Get Document API
  slug: docrocket-ai-get-document-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-get-document-api-openapi.yml
- filename: docrocket-ai-https-json-api-api-openapi.yml
  format: yaml
  label: docrocket-ai HTTPS JSON API
  slug: docrocket-ai-https-json-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-https-json-api-api-openapi.yml
- filename: docrocket-ai-list-brands-api-openapi.yml
  format: yaml
  label: docrocket-ai List Brands API
  slug: docrocket-ai-list-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-brands-api-openapi.yml
- filename: docrocket-ai-list-components-api-openapi.yml
  format: yaml
  label: docrocket-ai List Components API
  slug: docrocket-ai-list-components-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-components-api-openapi.yml
- filename: docrocket-ai-list-templates-api-openapi.yml
  format: yaml
  label: docrocket-ai List Templates API
  slug: docrocket-ai-list-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docrocket-ai/openapi/docrocket-ai-list-templates-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Docrocket Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: docrocket-ai secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: docrocket-ai
provider_slug: docrocket-ai
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Auth0 access token (DocRocket SPA audience) or DocRocket-issued API key JWT.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/docrocket-ai-openapi.json
  type: http
- description: OAuth 2.0 via DocRocket account. No API keys needed.
  flows:
  - authorizationUrl: https://app.docrocket.ai/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://app.docrocket.ai/oauth/token
  name: oauth2
  sources:
  - openapi/docrocket-ai-openapi.json
  type: oauth2
slug: docrocket-ai-authentication
source_filename: docrocket-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/docrocket-ai-openapi.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Auth0 access token (DocRocket SPA audience) or DocRocket-issued API key JWT.\n  sources:\n  - openapi/docrocket-ai-openapi.json\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.docrocket.ai/oauth/authorize\n    tokenUrl: https://app.docrocket.ai/oauth/token\n    scopes: 5\n  description: OAuth 2.0 via DocRocket account. No API keys needed.\n  sources:\n  - openapi/docrocket-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/docrocket-ai/authentication/docrocket-ai-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Document Generation
- Multi-tenant SaaS
- Brand Extraction
- PDF Generation
- AI Agents
- MCP Protocol
- SaaS Integration
---
