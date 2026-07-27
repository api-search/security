---
api_key_in: []
api_specs:
- filename: starlink-public-api-v2-openapi.json
  format: json
  label: Starlink Public API V2
  slug: starlink-public-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-public-api-v2-openapi.json
- filename: starlink-telemetry-asyncapi.yml
  format: yaml
  label: Starlink Telemetry Stream API
  slug: starlink-telemetry-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/asyncapi/starlink-telemetry-asyncapi.yml
- filename: starlink-public-api-v2-openapi.json
  format: json
  label: Starlink Mobile Data API
  slug: starlink-mobile-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-public-api-v2-openapi.json
- filename: starlink-public-api-v2-openapi.json
  format: json
  label: Starlink Aviation Flight Status API
  slug: starlink-aviation-flight-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/openapi/starlink-public-api-v2-openapi.json
auth_types:
- oauth2
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Starlink Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Starlink secures its APIs with oauth2, http, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Starlink
provider_slug: starlink
scheme_count: 4
schemes:
- applies_to: Starlink Public API V2 (account, service line, user terminal, router, billing, telemetry, mobile, flights)
  credential: clientId + secret minted as a "V2 Service Account" in the Starlink account settings page
  discovery: https://starlink.com/api/auth/.well-known/openid-configuration
  flow: clientCredentials
  id_token_signing_alg_values_supported:
  - RS384
  issuer: https://api.starlink.com/auth
  name: StarlinkServiceAccount
  presentation: 'Authorization: Bearer <access_token>'
  source: well-known/starlink-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  token_lifetime: ~15 minutes; reuse the token until a 401 is returned, then re-mint
  token_url: https://starlink.com/api/auth/connect/token
  type: oauth2
- applies_to: Starlink Space Traffic Coordination API (space-safety.starlink.com)
  credential: EC secp384r1 client key + a CSR signed by SpaceX into a client.crt
  docs: https://docs.space-safety.starlink.com/docs/api-keys
  environments:
  - https://staging.space-safety.starlink.com
  - https://space-safety.starlink.com
  name: SpaceSafetyClientCertificate
  onboarding: email space-safety-onboarding@spacex.com; access limited to satellite operators
  presentation: TLS client certificate (curl --key client.key --cert client.crt)
  type: mutualTLS
- applies_to: Starlink Local Device gRPC API (192.168.1.1:9000 router, 192.168.100.1:9200 user terminal)
  docs: https://starlink.readme.io/docs/device-api
  name: LocalDeviceNone
  rationale: no authentication because the gRPC server is only reachable on the local network
  type: none
- applies_to: Starlink Router Local HTTPS API (/starlinkrouter/)
  credential: enterprise-supplied TLS certificate + key configured on the router config, plus a CORS allowed-origins list
  docs: https://starlink.readme.io/docs/router-api
  name: RouterLocalHttpsTls
  note: the enterprise owns the certificate; the router serves the API on an operator-chosen domain
  type: mutualTLS
slug: starlink-authentication
source_filename: starlink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://starlink.readme.io/docs/authentication\ndocs: https://starlink.readme.io/docs/authentication\nnotes: >-\n  The downloadable Starlink Public API V2 OpenAPI (openapi/starlink-public-api-v2-openapi.json)\n  declares NO components.securitySchemes and no top-level security requirement, even though\n  every operation is authenticated. This profile was therefore harvested from the published\n  authentication guide, the API V2 Service Accounts guide, and the anonymous OIDC discovery\n  document, not derived from the spec. The per-operation authorization model is RBAC, carried\n  in each operation description as \"Required permission: <permission>, <View|Edit>\".\nsummary:\n  types: [oauth2, http, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [clientCredentials]\n  spec_declares_security_schemes: false\nschemes:\n- name: StarlinkServiceAccount\n  type: oauth2\n  applies_to: Starlink Public API V2 (account, service line, user\
  \ terminal, router, billing, telemetry, mobile, flights)\n  flow: clientCredentials\n  token_url: https://starlink.com/api/auth/connect/token\n  discovery: https://starlink.com/api/auth/.well-known/openid-configuration\n  issuer: https://api.starlink.com/auth\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post]\n  id_token_signing_alg_values_supported: [RS384]\n  credential: clientId + secret minted as a \"V2 Service Account\" in the Starlink account settings page\n  presentation: 'Authorization: Bearer <access_token>'\n  token_lifetime: ~15 minutes; reuse the token until a 401 is returned, then re-mint\n  source: well-known/starlink-openid-configuration.json\n- name: SpaceSafetyClientCertificate\n  type: mutualTLS\n  applies_to: Starlink Space Traffic Coordination API (space-safety.starlink.com)\n  docs: https://docs.space-safety.starlink.com/docs/api-keys\n  credential: EC secp384r1 client key + a CSR signed by SpaceX into a client.crt\n  presentation:\
  \ TLS client certificate (curl --key client.key --cert client.crt)\n  onboarding: email space-safety-onboarding@spacex.com; access limited to satellite operators\n  environments:\n  - https://staging.space-safety.starlink.com\n  - https://space-safety.starlink.com\n- name: LocalDeviceNone\n  type: none\n  applies_to: Starlink Local Device gRPC API (192.168.1.1:9000 router, 192.168.100.1:9200 user terminal)\n  docs: https://starlink.readme.io/docs/device-api\n  rationale: no authentication because the gRPC server is only reachable on the local network\n- name: RouterLocalHttpsTls\n  type: mutualTLS\n  applies_to: Starlink Router Local HTTPS API (/starlinkrouter/)\n  docs: https://starlink.readme.io/docs/router-api\n  credential: enterprise-supplied TLS certificate + key configured on the router config, plus a CORS allowed-origins list\n  note: the enterprise owns the certificate; the router serves the API on an operator-chosen domain\nservice_account_model:\n  docs: https://starlink.readme.io/docs/api-v2-service-accounts\n\
  \  scope: a V2 service account is bound to a Starlink ACCOUNT, not a user, and survives the creating user leaving\n  who_can_create: users holding the Admin or Service Account Management role\n  ceiling: a user cannot grant a service account a permission they do not themselves hold\n  limits:\n    service_accounts_per_account: 20\n    secrets_per_service_account: 20\n  rotation: secrets support an optional expiry; create new secrets then delete old ones to rotate\n  revocation: service accounts can be disabled but never deleted, to preserve traceability\n  mfa: service accounts are exempt from multi-factor authentication challenges\nauthorization:\n  model: role-based access control, declared per operation in the OpenAPI description\n  source: openapi/starlink-public-api-v2-openapi.json\n  permissions:\n  - Account information, View\n  - Account information, Edit\n  - Admin Only - API User Management, Edit\n  - Aviation flight status management, Edit\n  - Device command and configuration,\
  \ View\n  - Device command and configuration, Edit\n  - Device configuration assignment, Edit\n  - Device management, View\n  - Device management, Edit\n  - Device telemetry, View\n  - Financial, View\n  - Gated Feature - Starlink Mobile Data, View\n  - Managed Account Information, View\n  - Service plan, View\n  - Service plan, Edit\n  - User management, Edit\n  visibility_roles:\n  - Admin\n  - Technical\n  - Technical Read Only\n  - Technical Configuration\n  - Service Account Management\nfailure_modes:\n- status: 401\n  meaning: token expired or invalid; clear the cached token and mint a new one\n- status: 403\n  meaning: the service account lacks the required permission for this endpoint or resource (user_lacks_required_permission)\nrate_limits:\n  token_endpoint: 1000 authentication requests per 15 minutes per client IP\n  source: https://starlink.readme.io/docs/rate-limits-1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/starlink/refs/heads/main/authentication/starlink-authentication.yml
summary_line: oauth2/http/mutualTLS · 4 schemes
tags:
- Telecommunications
- United States
- Satellite
- Broadband
- Non-Terrestrial Networks
- Connectivity
- Device Management
- Telemetry
- Aviation
- Maritime
- Enterprise
---
