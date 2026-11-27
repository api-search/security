---
anonymous_access: false
api_key_in: []
api_specs:
- filename: listdrop-co-discovery-api-openapi.yml
  format: yaml
  label: ListDrop Discovery API
  slug: listdrop-co-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-discovery-api-openapi.yml
- filename: listdrop-co-feedback-api-openapi.yml
  format: yaml
  label: ListDrop Feedback API
  slug: listdrop-co-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-feedback-api-openapi.yml
- filename: listdrop-co-lists-api-openapi.yml
  format: yaml
  label: ListDrop Lists API
  slug: listdrop-co-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-lists-api-openapi.yml
- filename: listdrop-co-read-api-openapi.yml
  format: yaml
  label: ListDrop Read API
  slug: listdrop-co-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-read-api-openapi.yml
- filename: listdrop-co-webhooks-api-openapi.yml
  format: yaml
  label: ListDrop Webhooks API
  slug: listdrop-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/listdrop-co/openapi/listdrop-co-webhooks-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: ListDrop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ListDrop secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ListDrop
provider_slug: listdrop-co
scheme_count: 1
schemes:
- description: 'OAuth 2.1: authorization-code + PKCE (S256), public clients via RFC 7591 dynamic registration at https://www.listdrop.co/api/oauth/register. Metadata: https://www.listdrop.co/.well-known/oauth-authorization-server'
  flows:
  - authorizationUrl: https://www.listdrop.co/oauth/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://www.listdrop.co/api/oauth/token
  name: listdropOAuth
  sources:
  - openapi/listdrop-co-openapi.json
  type: oauth2
slug: listdrop-co-authentication
source_filename: listdrop-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/listdrop-co-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: listdropOAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.listdrop.co/oauth/authorize\n    tokenUrl: https://www.listdrop.co/api/oauth/token\n    scopes: 2\n  description: 'OAuth 2.1: authorization-code + PKCE (S256), public clients via RFC 7591 dynamic\n    registration at https://www.listdrop.co/api/oauth/register. Metadata: https://www.listdrop.co/.well-known/oauth-authorization-server'\n  sources:\n  - openapi/listdrop-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/listdrop-co/authentication/listdrop-co-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Social
- List
- Community
- Artificial Intelligence
- Platform
---
