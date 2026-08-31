---
api_key_in:
- header
api_specs:
- filename: airops-agent-api-openapi.yml
  format: yaml
  label: AirOps Agent API
  slug: airops-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-agent-api-openapi.yml
- filename: airops-analytics-api-openapi.yml
  format: yaml
  label: AirOps Analytics API
  slug: airops-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-analytics-api-openapi.yml
- filename: airops-answers-api-openapi.yml
  format: yaml
  label: AirOps Answers API
  slug: airops-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-answers-api-openapi.yml
- filename: airops-apps-api-openapi.yml
  format: yaml
  label: AirOps Apps API
  slug: airops-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-apps-api-openapi.yml
- filename: airops-brand-kits-api-openapi.yml
  format: yaml
  label: AirOps Brand Kits API
  slug: airops-brand-kits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-brand-kits-api-openapi.yml
- filename: airops-citations-api-openapi.yml
  format: yaml
  label: AirOps Citations API
  slug: airops-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-citations-api-openapi.yml
- filename: airops-competitors-api-openapi.yml
  format: yaml
  label: AirOps Competitors API
  slug: airops-competitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-competitors-api-openapi.yml
- filename: airops-content-updates-api-openapi.yml
  format: yaml
  label: AirOps Content Updates API
  slug: airops-content-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-content-updates-api-openapi.yml
- filename: airops-executions-api-openapi.yml
  format: yaml
  label: AirOps Executions API
  slug: airops-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-executions-api-openapi.yml
- filename: airops-files-api-openapi.yml
  format: yaml
  label: AirOps Files API
  slug: airops-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-files-api-openapi.yml
- filename: airops-grids-api-openapi.yml
  format: yaml
  label: AirOps Grids API
  slug: airops-grids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-grids-api-openapi.yml
- filename: airops-memory-stores-api-openapi.yml
  format: yaml
  label: AirOps Memory Stores API
  slug: airops-memory-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-memory-stores-api-openapi.yml
- filename: airops-personas-api-openapi.yml
  format: yaml
  label: AirOps Personas API
  slug: airops-personas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-personas-api-openapi.yml
- filename: airops-prompts-api-openapi.yml
  format: yaml
  label: AirOps Prompts API
  slug: airops-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-prompts-api-openapi.yml
- filename: airops-sentiment-theme-answers-api-openapi.yml
  format: yaml
  label: AirOps Sentiment Theme Answers API
  slug: airops-sentiment-theme-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-sentiment-theme-answers-api-openapi.yml
- filename: airops-tags-api-openapi.yml
  format: yaml
  label: AirOps Tags API
  slug: airops-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-tags-api-openapi.yml
- filename: airops-topics-api-openapi.yml
  format: yaml
  label: AirOps Topics API
  slug: airops-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-topics-api-openapi.yml
- filename: airops-web-pages-api-openapi.yml
  format: yaml
  label: AirOps Web Pages API
  slug: airops-web-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/openapi/airops-web-pages-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Airops Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AirOps secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AirOps
provider_slug: airops
scheme_count: 2
schemes:
- applies_to: https://api.airops.com/public_api/*
  description: Workspace API key presented as a Bearer token in the Authorization header for the REST API at api.airops.com. Keys are created and regenerated in Workspace Settings; regenerating immediately invalidates the previous key. Some execute endpoints also accept the key as an auth_token query parameter (webhook flows).
  format: Bearer [example key]
  header: Authorization
  location: header
  name: apiKeyBearer
  scheme: bearer
  type: http
- applies_to: https://app.airops.com/mcp
  description: OAuth 2.0 authorization-code flow (PKCE S256) used by the hosted MCP server at app.airops.com/mcp and OAuth clients. Discovery published at app.airops.com/.well-known/openid-configuration and /oauth-authorization-server.
  flows:
  - authorizationUrl: https://app.airops.com/oauth/authorize
    flow: authorizationCode
    introspectionUrl: https://app.airops.com/oauth/introspect
    pkce:
    - S256
    revocationUrl: https://app.airops.com/oauth/revoke
    scopes_supported:
    - api
    - openid
    - profile
    - email
    tokenUrl: https://app.airops.com/oauth/token
    userinfoUrl: https://app.airops.com/oauth/userinfo
  name: oauth2
  scheme: authorizationCode
  type: oauth2
slug: airops-authentication
source_filename: airops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.airops.com/api-reference/using-the-api/authentication\ndocs: https://docs.airops.com/api-reference/using-the-api/authentication\nalso_derived_from: openapi/airops-api-openapi.yml\nspec_confirmation: >-\n  Confirmed 2026-08-13 against the published OpenAPI harvested from\n  https://api.airops.com/public_api/openapi.yaml. The spec declares exactly one\n  security scheme — components.securitySchemes.bearer (type: http, scheme:\n  bearer) — applied per-operation, with a 401 \"Authentication error\" response on\n  all 42 operations. There is no document-level `security` default (flagged in\n  overlays/airops-api-overlay.yaml). The OpenAPI does NOT model the OAuth 2.0\n  scheme below: OAuth exists only for the hosted MCP server and is discoverable\n  solely through the /.well-known/ documents, so the two auth surfaces are\n  documented in different places and only this artifact unifies them.\nsummary:\n  types: [http,\
  \ oauth2]\n  api_key_in: [header]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: 'Bearer [example key]'\n  description: >-\n    Workspace API key presented as a Bearer token in the Authorization header for\n    the REST API at api.airops.com. Keys are created and regenerated in Workspace\n    Settings; regenerating immediately invalidates the previous key. Some execute\n    endpoints also accept the key as an auth_token query parameter (webhook flows).\n  applies_to: https://api.airops.com/public_api/*\n- name: oauth2\n  type: oauth2\n  scheme: authorizationCode\n  description: >-\n    OAuth 2.0 authorization-code flow (PKCE S256) used by the hosted MCP server at\n    app.airops.com/mcp and OAuth clients. Discovery published at\n    app.airops.com/.well-known/openid-configuration and /oauth-authorization-server.\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://app.airops.com/oauth/authorize\n    tokenUrl: https://app.airops.com/oauth/token\n    revocationUrl: https://app.airops.com/oauth/revoke\n    introspectionUrl: https://app.airops.com/oauth/introspect\n    userinfoUrl: https://app.airops.com/oauth/userinfo\n    scopes_supported: [api, openid, profile, email]\n    pkce: [S256]\n  applies_to: https://app.airops.com/mcp\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airops/refs/heads/main/authentication/airops-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Application
- Artificial Intelligence
- Content
- SEO
- AEO
- Answer Engine Optimization
- Generative Engine Optimization
- Workflows
- MCP
- Analytics
- Agent Skills
- OpenAPI
- Knowledge Base
- Content Marketing
- Citations
---
