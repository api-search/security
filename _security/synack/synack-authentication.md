---
api_key_in:
- header
api_specs:
- filename: synack-monolith-v1-openapi.yaml
  format: yaml
  label: Synack Enterprise API (Monolith v1)
  slug: synack-enterprise-api-monolith-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v1-openapi.yaml
- filename: synack-monolith-v2-openapi.yaml
  format: yaml
  label: Synack Client API (Monolith v2)
  slug: synack-client-api-monolith-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-monolith-v2-openapi.yaml
- filename: synack-assessment-v1-openapi.yaml
  format: yaml
  label: Synack Assessment Service
  slug: synack-assessment-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-assessment-v1-openapi.yaml
- filename: synack-asset-v2-openapi.yaml
  format: yaml
  label: Synack Asset Service
  slug: synack-asset-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-v2-openapi.yaml
- filename: synack-asset-discovery-openapi.yaml
  format: yaml
  label: Synack Asset Discovery Service
  slug: synack-asset-discovery-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-asset-discovery-openapi.yaml
- filename: synack-mission-v2-openapi.yaml
  format: yaml
  label: Synack Mission Service v2
  slug: synack-mission-service-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-mission-v2-openapi.yaml
- filename: synack-vulns-openapi.yaml
  format: yaml
  label: Synack Vulnerability Service
  slug: synack-vulnerability-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-vulns-openapi.yaml
- filename: synack-tagging-openapi.yaml
  format: yaml
  label: Synack Tagging Service
  slug: synack-tagging-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-tagging-openapi.yaml
- filename: synack-streaming-openapi.yaml
  format: yaml
  label: Synack Streaming Service
  slug: synack-streaming-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/openapi/synack-streaming-openapi.yaml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Synack Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Synack secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Synack
provider_slug: synack
scheme_count: 4
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synack-assessment-v1-openapi.yaml
  - openapi/synack-mission-v2-openapi.yaml
  - openapi/synack-monolith-v1-openapi.yaml
  - openapi/synack-monolith-v2-openapi.yaml
  - openapi/synack-streaming-openapi.yaml
  type: http
- flows:
  - authorizationUrl: login.synack.com
    flow: implicit
    scopes: 5
  name: OAuth2
  sources:
  - openapi/synack-asset-discovery-openapi.yaml
  - openapi/synack-asset-v2-openapi.yaml
  - openapi/synack-tagging-openapi.yaml
  - openapi/synack-vulns-openapi.yaml
  type: oauth2
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/synack-monolith-v1-openapi.yaml
  - openapi/synack-monolith-v2-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: X-Auth
  sources:
  - openapi/synack-monolith-v1-openapi.yaml
  - openapi/synack-monolith-v2-openapi.yaml
  type: apiKey
slug: synack-authentication
source_filename: synack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/synack-assessment-v1-openapi.yaml, openapi/synack-asset-discovery-openapi.yaml,\n  openapi/synack-asset-v2-openapi.yaml, openapi/synack-mission-v2-openapi.yaml, openapi/synack-monolith-v1-openapi.yaml,\n  openapi/synack-monolith-v2-openapi.yaml, openapi/synack-streaming-openapi.yaml, openapi/synack-tagging-openapi.yaml,\n  openapi/synack-vulns-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - implicit\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/synack-assessment-v1-openapi.yaml\n  - openapi/synack-mission-v2-openapi.yaml\n  - openapi/synack-monolith-v1-openapi.yaml\n  - openapi/synack-monolith-v2-openapi.yaml\n  - openapi/synack-streaming-openapi.yaml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: login.synack.com\n    scopes: 5\n  sources:\n  - openapi/synack-asset-discovery-openapi.yaml\n\
  \  - openapi/synack-asset-v2-openapi.yaml\n  - openapi/synack-tagging-openapi.yaml\n  - openapi/synack-vulns-openapi.yaml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/synack-monolith-v1-openapi.yaml\n  - openapi/synack-monolith-v2-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Auth\n  sources:\n  - openapi/synack-monolith-v1-openapi.yaml\n  - openapi/synack-monolith-v2-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synack/refs/heads/main/authentication/synack-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Company
- Security
- Penetration Testing
- Vulnerability Management
- Attack Surface Management
- Crowdsourced Security
- Compliance
- API
---
