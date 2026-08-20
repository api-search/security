---
api_key_in: []
api_specs:
- filename: drchrono-administrative-api-openapi.yml
  format: yaml
  label: drchrono Administrative API
  slug: drchrono-administrative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-administrative-api-openapi.yml
- filename: drchrono-audit-api-openapi.yml
  format: yaml
  label: drchrono Audit API
  slug: drchrono-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-audit-api-openapi.yml
- filename: drchrono-availability-api-openapi.yml
  format: yaml
  label: drchrono Availability API
  slug: drchrono-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-availability-api-openapi.yml
- filename: drchrono-billing-api-openapi.yml
  format: yaml
  label: drchrono Billing API
  slug: drchrono-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-billing-api-openapi.yml
- filename: drchrono-clinical-api-openapi.yml
  format: yaml
  label: drchrono Clinical API
  slug: drchrono-clinical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-clinical-api-openapi.yml
- filename: drchrono-practice-management-api-openapi.yml
  format: yaml
  label: drchrono Practice Management API
  slug: drchrono-practice-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/openapi/drchrono-practice-management-api-openapi.yml
auth_types:
- oauth2
description: DrChrono runs two independent OAuth 2.0 estates that share no tokens, no scopes and no discovery surface. The proprietary REST v4 API authenticates against app.drchrono.com with a DrChrono-specific scope vocabulary and a hard 48-hour access-token lifetime. The ONC-certified SMART on FHIR R4 API authenticates against a separate EverHealth-hosted authorization server with SMART scopes, PKCE and OIDC. A token from one is not valid against the other.
kind: authentication
layout: security
method: searched
name: Drchrono Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
- implicit
- deviceCode
overview: drchrono secures its APIs with oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, refreshToken, implicit, and deviceCode flow(s).
provider_name: drchrono
provider_slug: drchrono
scheme_count: 4
schemes:
- client_registration:
    console: https://app.drchrono.com/api-management/
    issues: client id, client secret
    note: A free DrChrono account is enough to create an API application.
    path_in_app: Account > Other Settings > API
    requires: application name, one or more redirect URIs
    self_serve: true
  declared_in: openapi/_original/drchrono-rest-api-openapi-schema.json
  discovery:
    note: No RFC 8414 or OIDC metadata document is published for this authorization server. https://app.drchrono.com/.well-known/oauth-authorization-server returned 404 on 2026-08-14. Endpoints exist only in prose.
    oauth_authorization_server: false
    openid_configuration: false
  flows:
  - authorizationUrl: https://app.drchrono.com/o/authorize/
    flow: authorizationCode
    revocationUrl: https://app.drchrono.com/o/revoke_token
    scope_artifact: scopes/drchrono-scopes.yml
    scopes: 22
    tokenUrl: https://app.drchrono.com/o/token/
  name: drchrono_oauth2
  permission_gate:
    description: 'Scopes alone do not authorise access. DrChrono enforces a second, independent gate: a primary user must grant the corresponding permission to the user inside the DrChrono web app. A token carrying the correct scope still returns 403 when the in-app permission is absent, and this is the single most common integration failure on this API.'
    example: The share_communications permission controls whether /api/messages and /api/lab_results share practice communication data over the API; it is editable only by DrChrono employees on request to api@drchrono.com.
  scope_default_hazard: Omitting the scope parameter on the authorize call requests ALL scopes. DrChrono's own documentation advises requesting only what is needed; the default is maximal, not minimal.
  sources:
  - https://app.drchrono.com/api-docs/
  - https://app.drchrono.com/api-docs/tutorial/
  - openapi/_original/drchrono-rest-api-openapi-schema.json
  surface: REST v4 API (app.drchrono.com)
  token:
    access_token_lifetime_hours: 48
    authorization_code_lifetime: Very short. DrChrono warns the code "expires extremely quickly" and that the exchange must happen before the redirect page is rendered to the user.
    refresh: refresh_token grant against the same token endpoint, omitting redirect_uri
    rotation: not documented
    transport: 'Authorization: Bearer <access_token>'
  type: oauth2
- client_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  client_registration:
    dynamic_client_registration: false
    note: The registration endpoint is a permissions console. DrChrono states only EHR vendor admins can add a client app, supplying application URL, redirect URL, logout URL, scope list, application name and OAuth flow.
    self_serve: false
  declared_in: well-known/drchrono-fhir-smart-configuration.json
  discovery:
    openid_configuration: https://drchrono-fhir.everhealthsoftware.com/core/.well-known/openid-configuration
    smart_configuration: https://drchrono-fhirpresentation.everhealthsoftware.com/fhir/drchrono/498711/r4/.well-known/smart-configuration
    status: both returned 200 on 2026-08-14 and are saved verbatim under well-known/
  endpoints:
    introspection: https://drchrono-fhir.everhealthsoftware.com/core/connect/introspect
    registration: https://drchrono-fhir.everhealthsoftware.com/core/permissions
    revocation: https://drchrono-fhir.everhealthsoftware.com/core/connect/revocation
  flows:
  - aud_parameter: the FHIR base URL must be passed as aud on the authorize call
    authorizationUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/authorize
    flow: authorizationCode
    pkce: required in practice (S256 is the only advertised challenge method)
    tokenUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/token
  - client_assertion: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
    flow: clientCredentials
    tokenUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/token
    used_for: FHIR Bulk Data Export with scope system/*.read
  - flow: refreshToken
  - flow: implicit
  - flow: deviceCode
    grant: urn:ietf:params:oauth:grant-type:device_code
  issuer: https://drchrono-fhir.everhealthsoftware.com/core
  name: drchrono_smart_fhir
  openid_connect: true
  scope_artifact: scopes/drchrono-fhir-smart-scopes.yml
  scopes: 233
  sources:
  - well-known/drchrono-fhir-smart-configuration.json
  - well-known/drchrono-fhir-openid-configuration.json
  - https://drchrono-fhirpresentation.everhealthsoftware.com/drchrono/498711/r4/Home/ApiDocumentation
  surface: SMART on FHIR R4 API (drchrono-fhirpresentation.everhealthsoftware.com)
  type: oauth2
- algorithm: HS256
  claims:
  - doctor_id
  - patient_id
  - practice_id
  - iat
  description: DrChrono appends a signed JWT to the iframe src when rendering a third-party application inside the patient chart or clinical note page. The JWT signs the context parameters so the embedding application can verify it is being loaded by an authorised DrChrono user. Because same-origin policy blocks postMessage-free data exchange, the JWT is the only trusted context channel.
  guidance: Validate the JWT with a vetted library and use ONLY the claims extracted from it — never the raw query parameters. DrChrono's own example allows 60 seconds of clock drift.
  key: the API application's client_secret
  name: drchrono_iframe_jwt
  source: https://app.drchrono.com/api-docs/
  surface: Embedded iframe applications inside the DrChrono patient chart and clinical note
  type: jwt
- description: Webhook deliveries carry the shared secret in a header rather than an HMAC of the request body, so the header authenticates the sender but attests nothing about payload integrity. A separate HMAC-SHA256 challenge/response is used once at webhook creation and whenever the callback URL changes.
  header: X-drchrono-signature
  name: drchrono_webhook_secret
  source: https://app.drchrono.com/api-docs/
  surface: Outbound webhook deliveries
  type: shared secret
  verification_handshake: HMAC-SHA256 hex digest of the msg query parameter, keyed by the webhook secret token
slug: drchrono-authentication
source_filename: drchrono-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://app.drchrono.com/api-docs/\ndocs: https://app.drchrono.com/api-docs/tutorial/\nname: drchrono Authentication\ndescription: >-\n  DrChrono runs two independent OAuth 2.0 estates that share no tokens, no scopes and no discovery\n  surface. The proprietary REST v4 API authenticates against app.drchrono.com with a DrChrono-specific\n  scope vocabulary and a hard 48-hour access-token lifetime. The ONC-certified SMART on FHIR R4 API\n  authenticates against a separate EverHealth-hosted authorization server with SMART scopes, PKCE and\n  OIDC. A token from one is not valid against the other.\n\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken, implicit, deviceCode]\n  api_keys: false\n  basic_auth: false\n  mutual_tls: false\n  openid_connect: true\n  openid_connect_scope: FHIR surface only\n\nschemes:\n  - name: drchrono_oauth2\n    surface: REST v4 API (app.drchrono.com)\n\
  \    type: oauth2\n    declared_in: openapi/_original/drchrono-rest-api-openapi-schema.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://app.drchrono.com/o/authorize/\n        tokenUrl: https://app.drchrono.com/o/token/\n        revocationUrl: https://app.drchrono.com/o/revoke_token\n        scopes: 22\n        scope_artifact: scopes/drchrono-scopes.yml\n    token:\n      transport: 'Authorization: Bearer <access_token>'\n      access_token_lifetime_hours: 48\n      refresh: refresh_token grant against the same token endpoint, omitting redirect_uri\n      authorization_code_lifetime: >-\n        Very short. DrChrono warns the code \"expires extremely quickly\" and that the exchange must\n        happen before the redirect page is rendered to the user.\n      rotation: not documented\n    client_registration:\n      self_serve: true\n      console: https://app.drchrono.com/api-management/\n      path_in_app: Account > Other Settings > API\n      requires:\
  \ application name, one or more redirect URIs\n      issues: client id, client secret\n      note: A free DrChrono account is enough to create an API application.\n    scope_default_hazard: >-\n      Omitting the scope parameter on the authorize call requests ALL scopes. DrChrono's own\n      documentation advises requesting only what is needed; the default is maximal, not minimal.\n    permission_gate:\n      description: >-\n        Scopes alone do not authorise access. DrChrono enforces a second, independent gate: a primary\n        user must grant the corresponding permission to the user inside the DrChrono web app. A token\n        carrying the correct scope still returns 403 when the in-app permission is absent, and this is\n        the single most common integration failure on this API.\n      example: >-\n        The share_communications permission controls whether /api/messages and /api/lab_results share\n        practice communication data over the API; it is editable only by\
  \ DrChrono employees on request\n        to api@drchrono.com.\n    discovery:\n      oauth_authorization_server: false\n      openid_configuration: false\n      note: >-\n        No RFC 8414 or OIDC metadata document is published for this authorization server.\n        https://app.drchrono.com/.well-known/oauth-authorization-server returned 404 on 2026-08-14.\n        Endpoints exist only in prose.\n    sources:\n      - https://app.drchrono.com/api-docs/\n      - https://app.drchrono.com/api-docs/tutorial/\n      - openapi/_original/drchrono-rest-api-openapi-schema.json\n\n  - name: drchrono_smart_fhir\n    surface: SMART on FHIR R4 API (drchrono-fhirpresentation.everhealthsoftware.com)\n    type: oauth2\n    openid_connect: true\n    issuer: https://drchrono-fhir.everhealthsoftware.com/core\n    declared_in: well-known/drchrono-fhir-smart-configuration.json\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/authorize\n\
  \        tokenUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/token\n        pkce: required in practice (S256 is the only advertised challenge method)\n        aud_parameter: 'the FHIR base URL must be passed as aud on the authorize call'\n      - flow: clientCredentials\n        tokenUrl: https://drchrono-fhir.everhealthsoftware.com/core/connect/token\n        client_assertion: 'urn:ietf:params:oauth:client-assertion-type:jwt-bearer'\n        used_for: FHIR Bulk Data Export with scope system/*.read\n      - flow: refreshToken\n      - flow: implicit\n      - flow: deviceCode\n        grant: 'urn:ietf:params:oauth:grant-type:device_code'\n    endpoints:\n      introspection: https://drchrono-fhir.everhealthsoftware.com/core/connect/introspect\n      revocation: https://drchrono-fhir.everhealthsoftware.com/core/connect/revocation\n      registration: https://drchrono-fhir.everhealthsoftware.com/core/permissions\n    client_auth_methods: [client_secret_basic, client_secret_post,\
  \ private_key_jwt]\n    scopes: 233\n    scope_artifact: scopes/drchrono-fhir-smart-scopes.yml\n    client_registration:\n      self_serve: false\n      dynamic_client_registration: false\n      note: >-\n        The registration endpoint is a permissions console. DrChrono states only EHR vendor admins can\n        add a client app, supplying application URL, redirect URL, logout URL, scope list, application\n        name and OAuth flow.\n    discovery:\n      smart_configuration: https://drchrono-fhirpresentation.everhealthsoftware.com/fhir/drchrono/498711/r4/.well-known/smart-configuration\n      openid_configuration: https://drchrono-fhir.everhealthsoftware.com/core/.well-known/openid-configuration\n      status: both returned 200 on 2026-08-14 and are saved verbatim under well-known/\n    sources:\n      - well-known/drchrono-fhir-smart-configuration.json\n      - well-known/drchrono-fhir-openid-configuration.json\n      - https://drchrono-fhirpresentation.everhealthsoftware.com/drchrono/498711/r4/Home/ApiDocumentation\n\
  \n  - name: drchrono_iframe_jwt\n    surface: Embedded iframe applications inside the DrChrono patient chart and clinical note\n    type: jwt\n    algorithm: HS256\n    key: the API application's client_secret\n    claims: [doctor_id, patient_id, practice_id, iat]\n    description: >-\n      DrChrono appends a signed JWT to the iframe src when rendering a third-party application inside\n      the patient chart or clinical note page. The JWT signs the context parameters so the embedding\n      application can verify it is being loaded by an authorised DrChrono user. Because same-origin\n      policy blocks postMessage-free data exchange, the JWT is the only trusted context channel.\n    guidance: >-\n      Validate the JWT with a vetted library and use ONLY the claims extracted from it — never the raw\n      query parameters. DrChrono's own example allows 60 seconds of clock drift.\n    source: https://app.drchrono.com/api-docs/\n\n  - name: drchrono_webhook_secret\n    surface: Outbound\
  \ webhook deliveries\n    type: shared secret\n    header: X-drchrono-signature\n    verification_handshake: HMAC-SHA256 hex digest of the msg query parameter, keyed by the webhook secret token\n    description: >-\n      Webhook deliveries carry the shared secret in a header rather than an HMAC of the request body,\n      so the header authenticates the sender but attests nothing about payload integrity. A separate\n      HMAC-SHA256 challenge/response is used once at webhook creation and whenever the callback URL\n      changes.\n    source: https://app.drchrono.com/api-docs/\n\nfindings:\n  - >-\n    Neither DrChrono OAuth surface publishes RFC 8414 authorization-server metadata for the REST API;\n    only the FHIR estate is discoverable.\n  - >-\n    The 48-hour access token is short for a background integration and there is no client-credentials\n    flow on the REST API — every REST integration is bound to a human user's authorization and must\n    keep a refresh token alive indefinitely.\n\
  \  - >-\n    PKCE is available on the FHIR surface and absent from the REST surface's documentation.\n  - >-\n    The scope/permission double gate is the defining characteristic of DrChrono auth and is invisible\n    in the OpenAPI. It is documented in prose only.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/drchrono/refs/heads/main/authentication/drchrono-authentication.yml
summary_line: oauth2 · 4 schemes
tags:
- EHR
- Electronic Health Records
- Healthcare
- Medical Records
- Practice Management
- HIPAA
- Appointments
- Billing
- Prescriptions
- Lab Integration
- FHIR
- SMART on FHIR
- USCDI
- Interoperability
- Webhook
- Authentication
- ONC Certified
- Telehealth
- Revenue Cycle Management
---
