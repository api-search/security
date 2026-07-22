---
api_key_in: []
api_specs:
- filename: servicechannel-service-automation-openapi-original.json
  format: json
  label: ServiceChannel Service Automation API
  slug: servicechannel-service-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-service-automation-openapi-original.json
- filename: servicechannel-fixxbook-openapi-original.json
  format: json
  label: ServiceChannel Fixxbook API
  slug: servicechannel-fixxbook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/openapi/servicechannel-fixxbook-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Servicechannel Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: ServiceChannel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: ServiceChannel
provider_slug: servicechannel
scheme_count: 1
schemes:
- description: 'OAuth2 authorization-code grant. Register an application to obtain a client_id and client_secret, then exchange for a bearer access token sent as Authorization: Bearer <token>. No granular OAuth scopes are declared; access is governed by the authenticated user''s ServiceChannel security permissions (error code 504 = call rejected by security permissions).'
  flows:
  - authorizationUrl: https://login.servicechannel.com/oauth/authorize
    flow: authorizationCode
    sandbox_authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize
    sandbox_tokenUrl: https://sb2login.servicechannel.com/oauth/token
    scopes: 0
    tokenUrl: https://login.servicechannel.com/oauth/token
  name: oauth2
  sources:
  - openapi/servicechannel-fixxbook-openapi-original.json
  - openapi/servicechannel-service-automation-openapi-original.json
  type: oauth2
slug: servicechannel-authentication
source_filename: servicechannel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/servicechannel-fixxbook-openapi-original.json, openapi/servicechannel-service-automation-openapi-original.json\ndocs: https://developer.servicechannel.com/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.servicechannel.com/oauth/authorize\n    tokenUrl: https://login.servicechannel.com/oauth/token\n    sandbox_authorizationUrl: https://sb2login.servicechannel.com/oauth/authorize\n    sandbox_tokenUrl: https://sb2login.servicechannel.com/oauth/token\n    scopes: 0\n  description: >-\n    OAuth2 authorization-code grant. Register an application to obtain a\n    client_id and client_secret, then exchange for a bearer access token sent as\n    Authorization: Bearer <token>. No granular OAuth scopes are declared; access\n    is governed by the authenticated user's ServiceChannel security\
  \ permissions\n    (error code 504 = call rejected by security permissions).\n  sources:\n  - openapi/servicechannel-fixxbook-openapi-original.json\n  - openapi/servicechannel-service-automation-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servicechannel/refs/heads/main/authentication/servicechannel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Services
- Facilities Management
- Work Orders
- Field Service
- Maintenance
- Asset Management
- Service Providers
- Invoicing
---
