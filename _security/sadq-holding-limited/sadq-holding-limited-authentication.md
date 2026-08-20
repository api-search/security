---
api_key_in: []
api_specs:
- filename: sadq-holding-limited-archiving-delegations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Archiving & Delegations API
  slug: sadq-holding-limited-archiving-delegations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-archiving-delegations-api-openapi.yml
- filename: sadq-holding-limited-authentication-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Authentication API
  slug: sadq-holding-limited-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-authentication-api-openapi.yml
- filename: sadq-holding-limited-configuration-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Configuration API
  slug: sadq-holding-limited-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-configuration-api-openapi.yml
- filename: sadq-holding-limited-documents-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Documents API
  slug: sadq-holding-limited-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-documents-api-openapi.yml
- filename: sadq-holding-limited-envelopes-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Envelopes API
  slug: sadq-holding-limited-envelopes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-envelopes-api-openapi.yml
- filename: sadq-holding-limited-esign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited eSign API
  slug: sadq-holding-limited-esign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-esign-api-openapi.yml
- filename: sadq-holding-limited-invitations-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Invitations API
  slug: sadq-holding-limited-invitations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-invitations-api-openapi.yml
- filename: sadq-holding-limited-kyb-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited KYB API
  slug: sadq-holding-limited-kyb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-kyb-api-openapi.yml
- filename: sadq-holding-limited-reports-requests-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Reports & Requests API
  slug: sadq-holding-limited-reports-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-reports-requests-api-openapi.yml
- filename: sadq-holding-limited-sign-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Sign API
  slug: sadq-holding-limited-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-sign-api-openapi.yml
- filename: sadq-holding-limited-templates-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Templates API
  slug: sadq-holding-limited-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-templates-api-openapi.yml
- filename: sadq-holding-limited-users-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Users API
  slug: sadq-holding-limited-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-users-api-openapi.yml
- filename: sadq-holding-limited-webhooks-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Webhooks API
  slug: sadq-holding-limited-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-webhooks-api-openapi.yml
- filename: sadq-holding-limited-workflows-api-openapi.yml
  format: yaml
  label: Sadq Holding Limited Workflows API
  slug: sadq-holding-limited-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/openapi/sadq-holding-limited-workflows-api-openapi.yml
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sadq Holding Limited Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Sadq Holding Limited secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Sadq Holding Limited
provider_slug: sadq-holding-limited
scheme_count: 2
schemes:
- authorization_server: https://identity.sadq.sa
  flow: clientCredentials
  introspection_url: https://identity.sadq.sa/connect/introspect
  name: OAuth2ClientCredentials
  note: Agents/services register at https://sadq.sa/register for a client_id + client_secret, then exchange them via the client_credentials grant for a Bearer JWT (RS256). Documented in auth.md and the RFC 8414 / RFC 9728 discovery documents on docs.sadq.sa.
  revocation_url: https://identity.sadq.sa/connect/revocation
  scopes:
  - Integrationscope
  sources:
  - https://docs.sadq.sa/.well-known/oauth-authorization-server
  - https://docs.sadq.sa/auth.md
  token_url: https://identity.sadq.sa/connect/token
  type: oauth2
- bearerFormat: JWT
  name: BearerAuth
  note: Every API operation in the OpenAPI declares BearerAuth (JWT). The token is obtained via the OAuth2 client_credentials flow above, or from the legacy POST /Authentication/Authority/Token endpoint (Basic Auth with Client ID / Client Secret + form body grant_type=integration).
  scheme: bearer
  sources:
  - openapi/sadq-holding-limited-openapi-original.json
  type: http
slug: sadq-holding-limited-authentication
source_filename: sadq-holding-limited-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sadq-holding-limited-openapi-original.json\ndocs: https://docs.sadq.sa/auth.md\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  bearer_format: JWT\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://identity.sadq.sa/connect/token\n  authorization_server: https://identity.sadq.sa\n  scopes:\n  - Integrationscope\n  revocation_url: https://identity.sadq.sa/connect/revocation\n  introspection_url: https://identity.sadq.sa/connect/introspect\n  note: >-\n    Agents/services register at https://sadq.sa/register for a client_id +\n    client_secret, then exchange them via the client_credentials grant for a\n    Bearer JWT (RS256). Documented in auth.md and the RFC 8414 / RFC 9728\n    discovery documents on docs.sadq.sa.\n  sources:\n  - https://docs.sadq.sa/.well-known/oauth-authorization-server\n  - https://docs.sadq.sa/auth.md\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  note: >-\n    Every API operation in the OpenAPI declares BearerAuth (JWT). The token is\n    obtained via the OAuth2 client_credentials flow above, or from the legacy\n    POST /Authentication/Authority/Token endpoint (Basic Auth with Client ID /\n    Client Secret + form body grant_type=integration).\n  sources:\n  - openapi/sadq-holding-limited-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sadq-holding-limited/refs/heads/main/authentication/sadq-holding-limited-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- E-Signature
- Digital Signature
- Identity
- KYB
- Document-Management
- Saudi Arabia
- Nafath
- Webhook
- Agent Ready
---
