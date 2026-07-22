---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Signiant Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Signiant secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Signiant
provider_slug: signiant
scheme_count: 1
schemes:
- applied_as: Authorization Bearer <access_token>
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  notes: A JSON Web Token (JWT) valid for one hour. All product APIs (Platform, Jet, Media Shuttle, Flight Deck) share this token endpoint. Clients must allow firewall egress to *.cloud.signiant.com.
  request_body: '{ "client_id": "<client_id>", "client_secret": "<client_secret>", "grant_type": "client_credentials" }'
  response: '{ "access_token": "<jwt>", "expires_in": 3600, "token_type": "Bearer" }'
  token_url: https://platform-api-service.services.cloud.signiant.com/oauth/token
  type: oauth2
slug: signiant-authentication
source_filename: signiant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.signiant.com/signiant-platform/getting-started/\ndocs: https://developer.signiant.com/signiant-platform/getting-started/\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  token_type: Bearer JWT\n  token_ttl_seconds: 3600\n  credential_issuance: Signiant Customer Care issues the client_id / client_secret pair (not self-serve)\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://platform-api-service.services.cloud.signiant.com/oauth/token\n  grant_type: client_credentials\n  request_body: '{ \"client_id\": \"<client_id>\", \"client_secret\": \"<client_secret>\", \"grant_type\": \"client_credentials\" }'\n  response: '{ \"access_token\": \"<jwt>\", \"expires_in\": 3600, \"token_type\": \"Bearer\" }'\n  applied_as: Authorization Bearer <access_token>\n  notes: >-\n    A JSON Web Token (JWT) valid for one hour. All product APIs (Platform,\
  \ Jet,\n    Media Shuttle, Flight Deck) share this token endpoint. Clients must allow\n    firewall egress to *.cloud.signiant.com.\nroles:\n  description: >-\n    Access is governed by product-scoped account roles bound to the credentials,\n    not by OAuth scopes. Roles seen in the docs:\n  values:\n  - product: Flight Deck\n    service_account_type: MANAGER_AND_AGENTS_SAAS\n    role: MANAGER_AND_AGENTS_SAAS_ADMIN\n  - product: Flight Deck\n    service_account_type: MANAGER_AND_AGENTS_SAAS\n    role: MANAGER_AND_AGENTS_SAAS_VIEW_ONLY\n  - product: Flight Deck\n    service_account_type: FLIGHT_GATEWAY\n    role: FLIGHT_GATEWAY_ADMIN\n  - product: Jet\n    service_account_type: S2S\n    role: S2S_ADMIN\n  - product: Jet\n    service_account_type: S2S\n    role: JET_VIEW_ONLY\n  - product: Media Engine\n    service_account_type: MEDIA_ENGINE\n    role: MEDIA_ENGINE_IT_ADMIN\n  - product: Media Engine\n    service_account_type: MEDIA_ENGINE\n    role: MEDIA_ENGINE_USER\n  - product: Media\
  \ Shuttle\n    service_account_type: MEDIA_SHUTTLE\n    role: MEDIA_SHUTTLE_IT_ADMIN\n  docs: https://developer.signiant.com/signiant-platform/user-roles-on-the-signiant-platform/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signiant/refs/heads/main/authentication/signiant-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- File Transfer
- Media Supply Chain
- Managed File Transfer
- Content Delivery
- Storage
- Webhooks
- OAuth
- Media & Entertainment
---
