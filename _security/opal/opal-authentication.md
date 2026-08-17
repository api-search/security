---
api_key_in:
- cookie
- header
api_specs:
- filename: opal-v2-openapi.yml
  format: yaml
  label: Opal API v2
  slug: opal-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v2-openapi.yml
- filename: opal-v3-openapi.yml
  format: yaml
  label: Opal API v3
  slug: opal-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v3-openapi.yml
- filename: opal-asgard-bff-openapi.yml
  format: yaml
  label: Opal Asgard BFF API
  slug: opal-asgard-bff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-asgard-bff-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Opal Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Opal secures its APIs with apiKey and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Opal
provider_slug: opal
scheme_count: 4
schemes:
- description: (Deprecated) This API also supports authentication via an API or session token set in the request headers.
  in: header
  name: api_key
  parameter: Session-Token
  sources:
  - openapi/opal-asgard-bff-openapi.yml
  - openapi/opal-v2-openapi.yml
  - openapi/opal-v3-openapi.yml
  type: apiKey
- description: This API uses OAuth 2.0 with the authorization code grant flow. You can find more detailed authentication instructions in the [Authentication Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0) section.
  flows:
  - authorizationUrl: /oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: /oauth2/token
  name: oauth2
  sources:
  - openapi/opal-v2-openapi.yml
  - openapi/opal-v3-openapi.yml
  type: oauth2
- description: 'The OAuth 2.0 client credentials flow is used for secure server-server

    requests when Opal does not need to associate a request with a particular

    Opal user. These anonymous requests are instead authorized based on the

    OAuth scope.'
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: /oauth/token
  name: anonymous_oauth
  sources:
  - openapi/opal-v3-openapi.yml
  type: oauth2
- description: 'A cookie set and read by the Monolith service that authorizes a non-opal

    user to view a presentation and the resources within it. Other services

    can rely on this cookie by asking Monolith to authenticate it.'
  in: cookie
  name: presentation_share_cookie
  parameter: share_token
  sources:
  - openapi/opal-v3-openapi.yml
  type: apiKey
slug: opal-authentication
source_filename: opal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/opal-asgard-bff-openapi.yml, openapi/opal-v2-openapi.yml, openapi/opal-v3-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - cookie\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Session-Token\n  description: (Deprecated) This API also supports authentication via an API or session token\n    set in the request headers.\n  sources:\n  - openapi/opal-asgard-bff-openapi.yml\n  - openapi/opal-v2-openapi.yml\n  - openapi/opal-v3-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: /oauth2/auth\n    tokenUrl: /oauth2/token\n    scopes: 1\n  description: This API uses OAuth 2.0 with the authorization code grant flow. You can find\n    more detailed authentication instructions in the [Authentication Strategies](/api/documentation#section/Authentication-Strategies/OAuth-2.0)\n\
  \    section.\n  sources:\n  - openapi/opal-v2-openapi.yml\n  - openapi/opal-v3-openapi.yml\n- name: anonymous_oauth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 1\n  description: |-\n    The OAuth 2.0 client credentials flow is used for secure server-server\n    requests when Opal does not need to associate a request with a particular\n    Opal user. These anonymous requests are instead authorized based on the\n    OAuth scope.\n  sources:\n  - openapi/opal-v3-openapi.yml\n- name: presentation_share_cookie\n  type: apiKey\n  in: cookie\n  parameter: share_token\n  description: |-\n    A cookie set and read by the Monolith service that authorizes a non-opal\n    user to view a presentation and the resources within it. Other services\n    can rely on this cookie by asking Monolith to authenticate it.\n  sources:\n  - openapi/opal-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/authentication/opal-authentication.yml
summary_line: apiKey/oauth2 · 4 schemes
tags:
- Company
- Consumer
- Marketing
- Content Planning
- Marketing Calendar
- Campaign Management
- Collaboration
- SaaS
- Content Marketing
- Editorial Calendar
- Workflow
- Approvals
- Digital Asset Management
- JSON:API
- OAuth 2.0
- OpenAPI
---
