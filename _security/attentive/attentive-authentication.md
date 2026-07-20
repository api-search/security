---
api_key_in: []
api_specs:
- filename: attentive-v1-openapi.yaml
  format: yaml
  label: Attentive API
  slug: attentive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v1-openapi.yaml
- filename: attentive-v2-openapi.yaml
  format: yaml
  label: Attentive API V2
  slug: attentive-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/openapi/attentive-v2-openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Attentive Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Attentive secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Attentive
provider_slug: attentive
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/attentive-v1-openapi.yaml
  - openapi/attentive-v2-openapi.yaml
  type: http
- description: This API uses OAuth 2 with the authorization code grant flow. [More info](https://docs.attentivemobile.com/pages/authentication/)
  flows:
  - authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens
  name: OAuthFlow
  sources:
  - openapi/attentive-v1-openapi.yaml
  - openapi/attentive-v2-openapi.yaml
  type: oauth2
slug: attentive-authentication
source_filename: attentive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/attentive-v1-openapi.yaml, openapi/attentive-v2-openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\n- name: OAuthFlow\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://ui-devel.attentivemobile.com/integrations/oauth-install?client_id={clientId}&redirect_uri={redirectUri}&scope={scope}\n    tokenUrl: https://api.attentivemobile.com/v1/authorization-codes/tokens\n    scopes: 6\n  description: This API uses OAuth 2 with the authorization code grant flow. [More\n    info](https://docs.attentivemobile.com/pages/authentication/)\n  sources:\n  - openapi/attentive-v1-openapi.yaml\n  - openapi/attentive-v2-openapi.yaml\ndocs: https://docs.attentive.com/docs/authentication\nnotes:\
  \ Bearer token in Authorization header. Private apps use a token generated in\n  the Attentive product; public apps use OAuth 2.0 authorization code grant (code\n  expires in 2 minutes) with install at ui.attentivemobile.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attentive/refs/heads/main/authentication/attentive-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Martech
- SMS Marketing
- Email Marketing
- Ecommerce
- Marketing Automation
- Subscribers
- Webhooks
- Customer Engagement
---
