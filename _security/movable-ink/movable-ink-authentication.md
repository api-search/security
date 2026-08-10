---
api_key_in: []
auth_types: []
description: Movable Ink runs two distinct authentication models. Machine-to-machine data ingestion into the Customer Data API uses HTTP Basic authentication with an Access Key ID and Access Secret issued per integration by the Movable Ink Solutions / Client Experience team, scoped to a per-tenant endpoint key embedded in the path. Human access to the Movable Ink Studio application uses OpenID Connect against an Auth0 tenant at auth.movableink.com. There is no self-service API key issuance and no public developer credential flow.
kind: authentication
layout: security
method: searched
name: Movable Ink Authentication
name_suffix: Authentication
oauth_flows: []
overview: Movable Ink declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Movable Ink
provider_slug: movable-ink
scheme_count: 2
schemes:
- credential_issuance: Not self-service. The Movable Ink Solutions Architect / Client Experience team issues the endpoint URL (with the tenant key in the path), the Access Key ID and the Access Secret after an event-mapping conversation. Movable Ink will supply the pair pre-base64-encoded on request.
  endpoint_pattern: https://collector.movableink-dmz.com/behavioral/{endpoint_key}
  evidence:
  - https://www.braze.com/docs/partners/message_personalization/dynamic_content/visual_and_interactive_content/movable_ink/customer_data_api
  - https://docs.tealium.com/server-side-connectors/movable-ink-connector/
  - https://segment.com/docs/connections/destinations/catalog/actions-movable-ink/
  header: Authorization
  id: customer_data_api_basic
  in: header
  rotation: not documented publicly
  scheme: basic
  surface: Customer Data API
  type: http
  value_format: Basic base64(access_key_id:access_secret)
- authorization_endpoint: https://auth.movableink.com/authorize
  device_authorization_endpoint: https://auth.movableink.com/oauth/device/code
  evidence:
  - https://auth.movableink.com/.well-known/openid-configuration
  - https://app.movableink.com/
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  - implicit
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  - urn:ietf:params:oauth:grant-type:jwt-bearer
  id: studio_oidc
  issuer: https://auth.movableink.com/
  jwks_uri: https://auth.movableink.com/.well-known/jwks.json
  mfa_challenge_endpoint: https://auth.movableink.com/mfa/challenge
  observed_app_flow: app.movableink.com 302s unauthenticated requests to auth.movableink.com/authorize with response_type=code and scope=openid profile email offline_access.
  openIdConnectUrl: https://auth.movableink.com/.well-known/openid-configuration
  pkce:
  - S256
  - plain
  provider: Auth0
  registration_endpoint: https://auth.movableink.com/oidc/register
  revocation_endpoint: https://auth.movableink.com/oauth/revoke
  surface: Movable Ink Studio web application (app.movableink.com)
  token_endpoint: https://auth.movableink.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://auth.movableink.com/userinfo
slug: movable-ink-authentication
source_filename: movable-ink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://auth.movableink.com/.well-known/openid-configuration\ndocs: https://www.braze.com/docs/partners/message_personalization/dynamic_content/visual_and_interactive_content/movable_ink/customer_data_api\nname: Movable Ink Authentication Profile\ndescription: >-\n  Movable Ink runs two distinct authentication models. Machine-to-machine data\n  ingestion into the Customer Data API uses HTTP Basic authentication with an\n  Access Key ID and Access Secret issued per integration by the Movable Ink\n  Solutions / Client Experience team, scoped to a per-tenant endpoint key\n  embedded in the path. Human access to the Movable Ink Studio application uses\n  OpenID Connect against an Auth0 tenant at auth.movableink.com. There is no\n  self-service API key issuance and no public developer credential flow.\nschemes:\n  - id: customer_data_api_basic\n    type: http\n    scheme: basic\n    surface: Customer Data API\n    in: header\n \
  \   header: Authorization\n    value_format: 'Basic base64(access_key_id:access_secret)'\n    endpoint_pattern: https://collector.movableink-dmz.com/behavioral/{endpoint_key}\n    credential_issuance: >-\n      Not self-service. The Movable Ink Solutions Architect / Client Experience\n      team issues the endpoint URL (with the tenant key in the path), the Access\n      Key ID and the Access Secret after an event-mapping conversation. Movable\n      Ink will supply the pair pre-base64-encoded on request.\n    rotation: not documented publicly\n    evidence:\n      - https://www.braze.com/docs/partners/message_personalization/dynamic_content/visual_and_interactive_content/movable_ink/customer_data_api\n      - https://docs.tealium.com/server-side-connectors/movable-ink-connector/\n      - https://segment.com/docs/connections/destinations/catalog/actions-movable-ink/\n  - id: studio_oidc\n    type: openIdConnect\n    surface: Movable Ink Studio web application (app.movableink.com)\n   \
  \ openIdConnectUrl: https://auth.movableink.com/.well-known/openid-configuration\n    issuer: https://auth.movableink.com/\n    provider: Auth0\n    authorization_endpoint: https://auth.movableink.com/authorize\n    token_endpoint: https://auth.movableink.com/oauth/token\n    userinfo_endpoint: https://auth.movableink.com/userinfo\n    jwks_uri: https://auth.movableink.com/.well-known/jwks.json\n    revocation_endpoint: https://auth.movableink.com/oauth/revoke\n    device_authorization_endpoint: https://auth.movableink.com/oauth/device/code\n    registration_endpoint: https://auth.movableink.com/oidc/register\n    mfa_challenge_endpoint: https://auth.movableink.com/mfa/challenge\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:token-exchange\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n    pkce: [S256,\
  \ plain]\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - none\n    observed_app_flow: >-\n      app.movableink.com 302s unauthenticated requests to\n      auth.movableink.com/authorize with response_type=code and\n      scope=openid profile email offline_access.\n    evidence:\n      - https://auth.movableink.com/.well-known/openid-configuration\n      - https://app.movableink.com/\nobservations:\n  - The Customer Data API endpoint key lives in the URL path, so the endpoint URL\n    is itself a secret and must be handled as one alongside the Basic credential.\n  - Basic authentication over TLS is the only documented server-to-server scheme;\n    there is no bearer token, HMAC request signing, or mTLS option published.\n  - The OIDC tenant advertises the full Auth0 default grant set, including the\n    resource-owner password grant, which is broader than the authorization-code\n    flow the Studio app actually\
  \ uses.\n  - No public developer signup issues API credentials; every credential path runs\n    through a Movable Ink team member.\ngaps:\n  - No public authentication reference on a Movable Ink-owned domain. The\n    authoritative guides live on support.movableink.com, which is customer-gated.\n  - No documented credential rotation or revocation procedure for Customer Data\n    API keys.\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n    - url: https://auth.movableink.com/.well-known/openid-configuration\n      status: 200\n    - url: https://app.movableink.com/\n      status: 302\n    - url: https://collector.movableink-dmz.com/behavioral/testkey\n      status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/movable-ink/refs/heads/main/authentication/movable-ink-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Marketing
- Personalization
- Email
- Customer Data
- Mobile SDK
- Artificial Intelligence
- Advertising Technology
- Content
- Events
---
