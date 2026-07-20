---
api_key_in: []
api_specs:
- filename: crowddev-cdp-public-openapi.yml
  format: yaml
  label: CDP Public API
  slug: cdp-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/openapi/crowddev-cdp-public-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Crowddev Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Crowd.dev secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Crowd.dev
provider_slug: crowddev
scheme_count: 2
schemes:
- description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only verifies the resulting token.'
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: https://linuxfoundation.auth0.com/oauth/token
  name: M2MBearer
  sources:
  - openapi/crowddev-cdp-akrites-external-openapi.yml
  - openapi/crowddev-cdp-public-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/crowddev-cdp-akrites-openapi.yml
  - openapi/crowddev-cdp-ossprey-openapi.yml
  - openapi/crowddev-cdp-packages-openapi.yml
  - openapi/crowddev-cdp-public-openapi.yml
  - openapi/crowddev-cdp-stewardships-openapi.yml
  - openapi/crowddev-cm-id-openapi.yml
  type: http
slug: crowddev-authentication
source_filename: crowddev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/crowddev-cdp-akrites-external-openapi.yml, openapi/crowddev-cdp-akrites-openapi.yml,\n  openapi/crowddev-cdp-ossprey-openapi.yml, openapi/crowddev-cdp-packages-openapi.yml, openapi/crowddev-cdp-public-openapi.yml,\n  openapi/crowddev-cdp-stewardships-openapi.yml, openapi/crowddev-cm-id-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: M2MBearer\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://linuxfoundation.auth0.com/oauth/token\n    scopes: 3\n  description: 'Auth0 machine-to-machine client-credentials flow. Akrites exchanges its client\n    ID/secret with Auth0 for a JWT and sends it as `Authorization: Bearer <token>`; CDP only\n    verifies the resulting token.'\n  sources:\n  - openapi/crowddev-cdp-akrites-external-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n\
  \  bearerFormat: JWT\n  sources:\n  - openapi/crowddev-cdp-akrites-openapi.yml\n  - openapi/crowddev-cdp-ossprey-openapi.yml\n  - openapi/crowddev-cdp-packages-openapi.yml\n  - openapi/crowddev-cdp-public-openapi.yml\n  - openapi/crowddev-cdp-stewardships-openapi.yml\n  - openapi/crowddev-cm-id-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowddev/refs/heads/main/authentication/crowddev-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Community
- Developer Relations
- Developer Data Platform
- Identity Resolution
- Open Source
- Community Data Platform
- Open Source Intelligence
---
