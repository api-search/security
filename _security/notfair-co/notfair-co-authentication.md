---
anonymous_access: false
api_key_in: []
api_specs:
- filename: notfair-co-health-api-openapi.yml
  format: yaml
  label: notfair-co Health API
  slug: notfair-co-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-health-api-openapi.yml
- filename: notfair-co-mcp-api-openapi.yml
  format: yaml
  label: notfair-co MCP API
  slug: notfair-co-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-mcp-api-openapi.yml
- filename: notfair-co-well-known-api-openapi.yml
  format: yaml
  label: notfair-co .well Known API
  slug: notfair-co-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/notfair-co/openapi/notfair-co-well-known-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Notfair Co Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: notfair-co secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: notfair-co
provider_slug: notfair-co
scheme_count: 1
schemes:
- description: Clients self-register at https://notfair.co/api/oauth/register (RFC 7591). The authorization step opens NotFair sign-in, where a person signs up or signs in, chooses a workspace and connects platforms; an agent cannot create the account or approve platform access for them. Authorization code with PKCE (S256) and RFC 8707 resource=https://notfair.co/api/mcp/notfair. Discover authorization server me
  flows:
  - authorizationUrl: https://notfair.co/api/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://notfair.co/api/oauth/token
  name: NotFairOAuth
  sources:
  - openapi/notfair-co-openapi.json
  type: oauth2
slug: notfair-co-authentication
source_filename: notfair-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/notfair-co-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: NotFairOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://notfair.co/api/oauth/authorize\n    tokenUrl: https://notfair.co/api/oauth/token\n    scopes: 0\n  description: Clients self-register at https://notfair.co/api/oauth/register (RFC 7591). The\n    authorization step opens NotFair sign-in, where a person signs up or signs in, chooses a\n    workspace and connects platforms; an agent cannot create the account or approve platform\n    access for them. Authorization code with PKCE (S256) and RFC 8707 resource=https://notfair.co/api/mcp/notfair.\n    Discover authorization server me\n  sources:\n  - openapi/notfair-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/notfair-co/authentication/notfair-co-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Advertising
- AI
- Marketing
- Automation
---
