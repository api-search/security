---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiable-companies-api-openapi.yml
  format: yaml
  label: Apiable Companies API
  slug: apiable-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-companies-api-openapi.yml
- filename: apiable-custom-properties-api-openapi.yml
  format: yaml
  label: Apiable Custom Properties API
  slug: apiable-custom-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-custom-properties-api-openapi.yml
- filename: apiable-docs-api-openapi.yml
  format: yaml
  label: Apiable Docs API
  slug: apiable-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-docs-api-openapi.yml
- filename: apiable-files-api-openapi.yml
  format: yaml
  label: Apiable Files API
  slug: apiable-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-files-api-openapi.yml
- filename: apiable-invitations-api-openapi.yml
  format: yaml
  label: Apiable Invitations API
  slug: apiable-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-invitations-api-openapi.yml
- filename: apiable-plans-api-openapi.yml
  format: yaml
  label: Apiable Plans API
  slug: apiable-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-plans-api-openapi.yml
- filename: apiable-products-api-openapi.yml
  format: yaml
  label: Apiable Products API
  slug: apiable-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-products-api-openapi.yml
- filename: apiable-subscriptions-api-openapi.yml
  format: yaml
  label: Apiable Subscriptions API
  slug: apiable-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-subscriptions-api-openapi.yml
- filename: apiable-teams-api-openapi.yml
  format: yaml
  label: Apiable Teams API
  slug: apiable-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-teams-api-openapi.yml
- filename: apiable-users-api-openapi.yml
  format: yaml
  label: Apiable Users API
  slug: apiable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-users-api-openapi.yml
- filename: apiable-webhooks-api-openapi.yml
  format: yaml
  label: Apiable Webhooks API
  slug: apiable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-webhooks-api-openapi.yml
- filename: apiable-server-info-api-openapi.yml
  format: yaml
  label: Apiable Server Info API
  slug: apiable-server-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/openapi/apiable-server-info-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apiable Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Apiable secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Apiable
provider_slug: apiable
scheme_count: 1
schemes:
- description: 'OAuth 2.0: Client Credentials'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://developer.apiable.io/api/oauth2/token
  name: oauth-cc
  sources:
  - openapi/apiable-platform-api-openapi.json
  type: oauth2
  x_receive_token_in: request-body
slug: apiable-authentication
source_filename: apiable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: openapi/apiable-platform-api-openapi.json\ndocs: https://www.apiable.io/docs/api-reference/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  bearer_token: true\n  api_key: false\n  applied_to_every_operation: true\nschemes:\n  - name: oauth-cc\n    type: oauth2\n    description: 'OAuth 2.0: Client Credentials'\n    flows:\n      - flow: clientCredentials\n        tokenUrl: https://developer.apiable.io/api/oauth2/token\n        scopes: 0\n    x_receive_token_in: request-body\n    sources: [openapi/apiable-platform-api-openapi.json]\nmodel: >-\n  A client id and client secret are exchanged at the tenant's own token endpoint\n  (<portal-host>/api/oauth2/token) for a JWT access token, which is then sent as a Bearer token on\n  every Platform API request. The spec's servers[] names https://developer.apiable.io because that\n  is Apiable's own reference portal; each customer calls their own portal host. The Apiable\n\
  \  GitHub Action exposes the same credential pair as api_key/api_secret plus an api_url.\nscopes_ref: scopes/apiable-scopes.yml\nnotes:\n  - Every one of the 66 published operations carries an explicit security requirement — there is no\n    unauthenticated operation, and every operation declares a 401 response.\n  - >-\n    Apiable does not provide an identity provider for portal end users; customers bring their own\n    over OpenID Connect (Entra ID, Google, Okta, Cognito, Auth0, Keycloak). That is the CONSUMER\n    auth surface of a customer's portal, not the Platform API's own auth.\n    Source https://www.apiable.io/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiable/refs/heads/main/authentication/apiable-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Amazon API Gateway
- API Gateway
- API Monetization
- API Portal
- Developer Experience
- Developer Portal
- Developer Tools
- Kong
- Platform
- Self-Service
---
