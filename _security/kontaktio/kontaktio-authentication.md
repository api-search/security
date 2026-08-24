---
api_key_in:
- header
api_specs:
- filename: kontaktio-device-management-openapi.yml
  format: yaml
  label: Kontakt.io Device Management API
  slug: kontaktio-device-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-device-management-openapi.yml
- filename: kontaktio-location-occupancy-openapi.yml
  format: yaml
  label: Kontakt.io Location & Occupancy API
  slug: kontaktio-location-occupancy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-location-occupancy-openapi.yml
- filename: kontaktio-spaces-openapi.yml
  format: yaml
  label: Kontakt.io Spaces API
  slug: kontaktio-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-spaces-openapi.yml
- filename: kontaktio-entity-management-openapi.yml
  format: yaml
  label: Kontakt.io Entity Management Integration API
  slug: kontaktio-entity-management-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/openapi/kontaktio-entity-management-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kontaktio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kontakt.io secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kontakt.io
provider_slug: kontaktio
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: 'Provide a JWT in the `Authorization: Bearer <token>` header. This is the standard authentication method for all API requests.


    Obtain a token via the OAuth2 Client Credentials flow from the Kontakt.io Keycloak identity provider.'
  name: bearer_token
  scheme: bearer
  sources:
  - openapi/kontaktio-device-management-openapi.yml
  - openapi/kontaktio-entity-management-openapi.yml
  type: http
- description: '**Deprecated — do not use for new integrations.** This method exists solely for backward compatibility and will be removed in a future release. Use JWT Bearer token authentication instead.


    If you still need an API Key: sign in to **Kio Cloud** > select **Users** > select **Security** > copy your **Server API Key**.'
  in: header
  name: api_key
  parameter: Api-Key
  sources:
  - openapi/kontaktio-device-management-openapi.yml
  - openapi/kontaktio-location-occupancy-openapi.yml
  - openapi/kontaktio-spaces-openapi.yml
  type: apiKey
slug: kontaktio-authentication
source_filename: kontaktio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: https://developer.kontakt.io/docs/dev-ctr-device-api/e1e3f6ec0e943-authentication, https://developer.kontakt.io/docs/dev-ctr-loc-occ-api/ZG9jOjE1NTkwMDU5-authentication,\n  https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow,\n  plus openapi/ (4 specs)\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: 'Provide a JWT in the `Authorization: Bearer <token>` header. This is the standard authentication\n    method for all API requests.\n\n\n    Obtain a token via the OAuth2 Client Credentials flow from the Kontakt.io Keycloak identity provider.'\n  sources:\n  - openapi/kontaktio-device-management-openapi.yml\n  - openapi/kontaktio-entity-management-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description:\
  \ '**Deprecated — do not use for new integrations.** This method exists solely for backward compatibility\n    and will be removed in a future release. Use JWT Bearer token authentication instead.\n\n\n    If you still need an API Key: sign in to **Kio Cloud** > select **Users** > select **Security** > copy\n    your **Server API Key**.'\n  sources:\n  - openapi/kontaktio-device-management-openapi.yml\n  - openapi/kontaktio-location-occupancy-openapi.yml\n  - openapi/kontaktio-spaces-openapi.yml\ndocs:\n- https://developer.kontakt.io/docs/dev-ctr-device-api/e1e3f6ec0e943-authentication\n- https://developer.kontakt.io/docs/dev-ctr-loc-occ-api/ZG9jOjE1NTkwMDU5-authentication\n- https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow\nprimary:\n  model: oauth2-client-credentials -> JWT bearer\n  idp: Keycloak (per-tenant realm)\n  token_endpoint: https://kc.cloud.{region}.kontakt.io/realms/{tenant}/protocol/openid-connect/token\n\
  \  grant_type: client_credentials\n  scope: profile email openid\n  token_type: Bearer\n  token_lifetime_seconds: 300\n  regions:\n  - us\n  - uk\n  tenant_note: '{tenant} is the account Tenant Name from the account URL https://{tenant}.app.cloud.{region}.kontakt.io'\n  authorization: Carried by the Keycloak client role integration-api, not by OAuth scopes. See scopes/kontaktio-scopes.yml.\n  client_provisioning: Integration API Clients are created in Kio Cloud under Users > Integration API by a\n    user holding the User Management integration-api role; Client ID is prefixed api-{companyId}-.\n  error_on_expiry: 401 Unauthorized. Refresh once and retry once; do not loop.\n  docs: https://developer.kontakt.io/docs/entity-management-integration-api/0255c5646ab01-authentication-o-auth2-client-credentials-flow\nlegacy:\n  model: api-key\n  header: Api-Key\n  status: deprecated\n  removal: Announced for removal in a future release; no date published.\n  provenance: Kio Cloud > Users > Security\
  \ > Server API Key (one per account user).\n  note: The deprecation is NOT uniformly applied. Only the Device Management spec marks api_key deprecated\n    and offers bearer_token alongside it. The Location & Occupancy and Spaces specs declare Api-Key as their\n    ONLY scheme, so a client written against the current published contracts still has to use the deprecated\n    mechanism for two of the four APIs.\nrequired_headers:\n- api: Device Management API\n  header: Accept\n  value: application/vnd.com.kontakt+json;version=10\n  required: true\n  note: Media-type versioning. Optional in practice but strongly recommended; an unsupported version returns\n    415.\n- api: Device Management API\n  header: Content-Type\n  value: application/x-www-form-urlencoded\n  required: true\n  applies_to: POST requests only\n- api: Device Management API\n  header: User-Agent\n  value: client software version\n  required: false\nhosts:\n- api: Device Management API\n  host: https://dm-api.cloud.{region}.kontakt.io\n\
  - api: Location & Occupancy API\n  host: https://apps.cloud.{region}.kontakt.io\n- api: Spaces API\n  host: https://api.cloud.{region}.kontakt.io/spaces\n- api: Entity Management Integration API\n  host: https://api.cloud.{region}.kontakt.io/entity-management\nmtls: false\nmfa_on_api: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kontaktio/refs/heads/main/authentication/kontaktio-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- IoT
- RTLS
- Healthcare
- Asset Tracking
- Location
- Occupancy
- Bluetooth
- Device Management
- Telemetry
- Sensors
- Streaming
---
