---
api_key_in:
- header
auth_types:
- http
- jwt
description: ''
kind: authentication
layout: security
method: searched
name: Embeddable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Embeddable secures its APIs with http and jwt across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Embeddable
provider_slug: embeddable
scheme_count: 2
schemes:
- docs: https://docs.embeddable.com/deployment/embeddables-api
  format: Bearer ${apiKey}
  header: Authorization
  location: header
  name: apiKeyBearer
  scheme: bearer
  type: http
  usage: Authenticates server-to-server calls to the Public APIs (tokens, embeddables, versions, schemas). Must never be exposed to client code.
- docs: https://docs.embeddable.com/deployment/tokens-api
  name: securityToken
  scheme: bearer
  type: jwt
  usage: Short-lived JWT returned by POST /api/v1/security-token, passed to the <em-beddable> web component (token attribute) to authorize a single embed and carry the row-level-security context for the viewing user/tenant.
slug: embeddable-authentication
source_filename: embeddable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.embeddable.com/deployment/tokens-api\ndocs: https://docs.embeddable.com/deployment/tokens-api\nnotes: >-\n  No OpenAPI is published, so this profile is captured from the docs rather than\n  derived from a spec. Two layers of auth: (1) a long-lived API key used server-side\n  to call the Public APIs, and (2) short-lived JWT \"security tokens\" minted by the\n  server and handed to the browser to authorize a specific embed.\nsummary:\n  types: [http, jwt]\n  api_key_in: [header]\n  server_side_only: true\nschemes:\n- name: apiKeyBearer\n  type: http\n  scheme: bearer\n  location: header\n  header: Authorization\n  format: \"Bearer ${apiKey}\"\n  usage: >-\n    Authenticates server-to-server calls to the Public APIs (tokens, embeddables,\n    versions, schemas). Must never be exposed to client code.\n  docs: https://docs.embeddable.com/deployment/embeddables-api\n- name: securityToken\n  type: jwt\n  scheme: bearer\n\
  \  usage: >-\n    Short-lived JWT returned by POST /api/v1/security-token, passed to the\n    <em-beddable> web component (token attribute) to authorize a single embed and\n    carry the row-level-security context for the viewing user/tenant.\n  docs: https://docs.embeddable.com/deployment/tokens-api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/embeddable/refs/heads/main/authentication/embeddable-authentication.yml
summary_line: http/jwt · 2 schemes
tags:
- Company
- Analytics
- Embedded Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Semantic Layer
- Developer Tools
- SaaS
---
