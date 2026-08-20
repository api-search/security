---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Locbox Labs Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: LocBox Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: LocBox Labs
provider_slug: locbox-labs
scheme_count: 1
schemes:
- api: Hownd Partner API
  authorization_server:
    discovery: well-known/locbox-labs-openid-configuration.json
    dpop_signing_alg_values_supported:
    - ES256
    grant_types_supported_includes_client_credentials: true
    id_token_signing_alg_values_supported:
    - HS256
    - RS256
    - PS256
    issuer: https://hownd.auth0.com/
    jwks_uri: https://hownd.auth0.com/.well-known/jwks.json
    token_endpoint_auth_methods_supported:
    - client_secret_basic
    - client_secret_post
    - private_key_jwt
    - none
  flows:
  - audience: https://partner-api.hownd.com
    flow: clientCredentials
    scopes: {}
    scopes_note: No API scopes are published for the partner audience. The tenant's OIDC discovery document advertises only standard OpenID Connect scopes (openid, profile, email, offline_access, phone, address), which govern end-user login to the Auth0 tenant rather than partner API authorization.
    tokenUrl: https://hownd.auth0.com/oauth/token
  name: HowndPartnerOAuth2
  sources:
  - https://github.com/LocBoxLabs/hownd-examples/blob/main/main.go
  - https://hownd.auth0.com/.well-known/openid-configuration
  type: oauth2
slug: locbox-labs-authentication
source_filename: locbox-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://github.com/LocBoxLabs/hownd-examples\ndocs: https://github.com/LocBoxLabs/hownd-examples/blob/main/README.md\nnote: >-\n  Hownd publishes no OpenAPI and no API reference, so this profile is not derived\n  from a spec. It is transcribed from the company's own first-party example\n  repository (LocBoxLabs is the Hownd GitHub organization, org email\n  dev@hownd.com) and corroborated against the live OAuth/OIDC discovery document\n  served by the company's Auth0 tenant, which was fetched anonymously.\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  bearer_token: true\n  tenant_scoping: X-Tenant-Id header\nschemes:\n- name: HowndPartnerOAuth2\n  type: oauth2\n  api: Hownd Partner API\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://hownd.auth0.com/oauth/token\n    audience: https://partner-api.hownd.com\n    scopes: {}\n    scopes_note: >-\n      No API scopes are published\
  \ for the partner audience. The tenant's OIDC\n      discovery document advertises only standard OpenID Connect scopes\n      (openid, profile, email, offline_access, phone, address), which govern\n      end-user login to the Auth0 tenant rather than partner API authorization.\n  authorization_server:\n    issuer: https://hownd.auth0.com/\n    discovery: well-known/locbox-labs-openid-configuration.json\n    jwks_uri: https://hownd.auth0.com/.well-known/jwks.json\n    token_endpoint_auth_methods_supported:\n    - client_secret_basic\n    - client_secret_post\n    - private_key_jwt\n    - none\n    grant_types_supported_includes_client_credentials: true\n    id_token_signing_alg_values_supported: [HS256, RS256, PS256]\n    dpop_signing_alg_values_supported: [ES256]\n  sources:\n  - https://github.com/LocBoxLabs/hownd-examples/blob/main/main.go\n  - https://hownd.auth0.com/.well-known/openid-configuration\nrequired_headers:\n- name: Authorization\n  value: Bearer [token]\n  required: true\n\
  \  source: https://github.com/LocBoxLabs/hownd-examples\n- name: Content-Type\n  value: application/json\n  required: true\n  source: https://github.com/LocBoxLabs/hownd-examples\n- name: X-Tenant-Id\n  value: value provided by Hownd\n  required: true\n  description: >-\n    Identifies which Hownd customer (merchant/business) the partner is acting on\n    behalf of. Hownd's own note - \"Arguably the Tenant ID could be used in the\n    HTTP path. Since it is security related, a header felt more appropriate.\"\n  source: https://github.com/LocBoxLabs/hownd-examples\ncredential_issuance:\n  self_service: false\n  process: >-\n    Client credentials and a per-merchant Tenant ID are issued by Hownd to\n    approved partners. There is no public sign-up, developer portal, or key\n    self-service page.\n  restrictions: >-\n    Hownd states the credentials \"must be secured and cannot be used in any\n    integration scenario other than server to server\" and \"must not be used in a\n    browser\
  \ or mobile application.\"\nx-evidence:\n- {url: 'https://github.com/LocBoxLabs/hownd-examples', http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://hownd.auth0.com/.well-known/openid-configuration', http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://hownd.auth0.com/.well-known/jwks.json', http_status: 200, fetched: '2026-08-13'}\n- {url: 'https://partner-api.hownd.com/', http_status: 404, fetched: '2026-08-13', note: 'host is live and answering (Go http server default 404); no route documented publicly'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locbox-labs/refs/heads/main/authentication/locbox-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketing
- Promotions
- Local Marketing
- Small Business
- Automation
- Coupons
- Email Marketing
- Loyalty
- Guest WiFi
- Family Entertainment
- Restaurant
---
