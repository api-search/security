---
api_key_in: []
api_specs:
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Messaging API
  slug: weave-hq-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Phone & Calls API
  slug: weave-hq-phone-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Contacts API
  slug: weave-hq-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Scheduling & Appointments API
  slug: weave-hq-scheduling-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Payments API
  slug: weave-hq-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Digital Forms API
  slug: weave-hq-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Reviews API
  slug: weave-hq-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
- filename: weave-hq-openapi.yml
  format: yaml
  label: Weave Events & Subscriptions API
  slug: weave-hq-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/openapi/weave-hq-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Weave Hq Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Weave secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Weave
provider_slug: weave-hq
scheme_count: 2
schemes:
- description: 'OAuth 2.0 access token issued by Weave''s OIDC provider. Authorization and token endpoints are served under https://auth.weaveconnect.com/oauth2/default (issuer https://oidc.weaveconnect.com). Present as `Authorization: Bearer ACCESS_TOKEN`.'
  flows:
  - authorizationUrl: https://auth.weaveconnect.com/oauth2/default/v1/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://auth.weaveconnect.com/oauth2/default/v1/token
  name: oauth2
  sources:
  - openapi/weave-hq-openapi.yml
  type: oauth2
- description: 'OAuth 2.0 bearer access token passed as `Authorization: Bearer ACCESS_TOKEN`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/weave-hq-openapi.yml
  type: http
slug: weave-hq-authentication
source_filename: weave-hq-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/weave-hq-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.weaveconnect.com/oauth2/default/v1/authorize\n    tokenUrl: https://auth.weaveconnect.com/oauth2/default/v1/token\n    scopes: 0\n  description: 'OAuth 2.0 access token issued by Weave''s OIDC provider. Authorization and token\n    endpoints are served under https://auth.weaveconnect.com/oauth2/default (issuer https://oidc.weaveconnect.com).\n    Present as `Authorization: Bearer ACCESS_TOKEN`.'\n  sources:\n  - openapi/weave-hq-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 bearer access token passed as `Authorization: Bearer ACCESS_TOKEN`.'\n  sources:\n  - openapi/weave-hq-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weave-hq/refs/heads/main/authentication/weave-hq-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Communication
- Healthcare
- VoIP
- Messaging
- SMS
- Scheduling
- Payments
- Reviews
- Dental
- Veterinary
---
