---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Zerto Authentication
name_suffix: Authentication
oauth_flows:
- password
- refreshToken
overview: Zerto secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password and refreshToken flow(s).
provider_name: Zerto
provider_slug: zerto
scheme_count: 2
schemes:
- client_id: zerto-client
  description: 'Zerto appliances (ZVM / Zerto Cloud Appliance / Zerto In-Cloud) embed a Keycloak identity provider. Clients obtain a bearer JWT via the OAuth2 Resource Owner Password Credentials grant, then send it as `Authorization: Bearer <token>` on every /v1 call.'
  flow: password
  grant_type: password
  name: KeycloakOAuth2
  notes: scope=openid is REQUIRED — without it the token is issued but /v1/* endpoints reject it. Lab/PoC installs may use the built-in `master` realm and `admin-cli` client instead of the production `zerto` realm / `zerto-client`.
  realm: zerto
  refresh: refresh_token (returned alongside access_token)
  required_scope: openid
  token_lifetime_seconds: 60
  token_url: https://<appliance>/auth/realms/zerto/protocol/openid-connect/token
  type: oauth2
- applied_to: all /v1 endpoints
  bearerFormat: JWT
  description: The Keycloak-issued access_token is presented on all /v1 API calls.
  name: BearerToken
  scheme: bearer
  type: http
slug: zerto-authentication
source_filename: zerto-authentication.yml
source_heading: Authentication Profile
source_url: https://github.com/ZertoPublic/zerto-api-quickstart
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/ZertoPublic/zerto-api-quickstart/blob/main/GETTING-STARTED.md\ndocs: https://help.zerto.com/\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [password, refreshToken]\nschemes:\n  - name: KeycloakOAuth2\n    type: oauth2\n    description: >-\n      Zerto appliances (ZVM / Zerto Cloud Appliance / Zerto In-Cloud) embed a Keycloak\n      identity provider. Clients obtain a bearer JWT via the OAuth2 Resource Owner Password\n      Credentials grant, then send it as `Authorization: Bearer <token>` on every /v1 call.\n    flow: password\n    token_url: https://<appliance>/auth/realms/zerto/protocol/openid-connect/token\n    grant_type: password\n    client_id: zerto-client\n    realm: zerto\n    required_scope: openid\n    token_lifetime_seconds: 60\n    refresh: refresh_token (returned alongside access_token)\n    notes: >-\n      scope=openid is REQUIRED — without it the token is\
  \ issued but /v1/* endpoints reject it.\n      Lab/PoC installs may use the built-in `master` realm and `admin-cli` client instead of\n      the production `zerto` realm / `zerto-client`.\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: The Keycloak-issued access_token is presented on all /v1 API calls.\n    applied_to: all /v1 endpoints\nsources:\n  - https://github.com/ZertoPublic/zerto-api-quickstart\n  - https://github.com/saackerman/ZertoSwaggerAPI (Zerto-API-10.0-U6-Reference.md)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerto/refs/heads/main/authentication/zerto-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Disaster Recovery
- Data Protection
- Backup
- Ransomware Resilience
- Business Continuity
- Cloud Migration
- Replication
- Infrastructure
---
