---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aignostics-public-api-openapi.yml
  format: yaml
  label: Aignostics Public API
  slug: aignostics-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/openapi/aignostics-public-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aignostics Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Aignostics secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Aignostics
provider_slug: aignostics
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://aignostics-platform.eu.auth0.com/authorize
    flow: authorizationCode
    note: Declared in the OpenAPI with an EMPTY scopes object. See scopes/aignostics-scopes.yml.
    scopes: 0
    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token
  - audience: https://aignostics-platform-samia
    deviceAuthorizationUrl: https://aignostics-platform.eu.auth0.com/oauth/device/code
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    note: Documented in the getting-started guide and supported by the tenant (grant_types_supported includes the device-code URN) but NOT declared in the OpenAPI securityScheme. A client generated from the spec alone will only know about the authorization-code flow, even though device code is the flow the docs actually teach and the one the SDK uses for headless and CLI callers.
    scope: offline_access
    standard: RFC 8628
    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token
  header: 'Authorization: Bearer {access_token}'
  in: header
  name: OAuth2AuthorizationCodeBearer
  sources:
  - openapi/aignostics-platform-api-openapi.json
  - https://aignostics.readthedocs.io/en/latest/get_started_api.html
  type: oauth2
slug: aignostics-authentication
source_filename: aignostics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  https://aignostics.readthedocs.io/en/latest/get_started_api.html,\n  https://aignostics-platform.eu.auth0.com/.well-known/openid-configuration,\n  openapi/aignostics-platform-api-openapi.json\ndocs: https://aignostics.readthedocs.io/en/latest/get_started_api.html\napi: Aignostics Platform API\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - deviceCode\n  anonymous_access: false\n  api_keys: false\n  statement: >-\n    \"There is no anonymous access and no organization-wide API key.\" Every call carries a per-user\n    OAuth bearer token; entitlement is evaluated against the user's organization.\nidentity_provider:\n  vendor: Auth0\n  tenant: aignostics-platform.eu.auth0.com\n  region: EU\n  issuer: https://aignostics-platform.eu.auth0.com/\n  discovery: https://aignostics-platform.eu.auth0.com/.well-known/openid-configuration\n  jwks_uri: https://aignostics-platform.eu.auth0.com/.well-known/jwks.json\n\
  \  enterprise_sso: true\n  mfa: mandatory\n  note: >-\n    The SDK README states enterprise SSO through Auth0 with mandatory two-factor authentication on\n    all user accounts, and SDK v1.3.0 added an organization parameter to the OAuth flow.\nschemes:\n- name: OAuth2AuthorizationCodeBearer\n  type: oauth2\n  in: header\n  header: 'Authorization: Bearer {access_token}'\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://aignostics-platform.eu.auth0.com/authorize\n    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token\n    scopes: 0\n    note: >-\n      Declared in the OpenAPI with an EMPTY scopes object. See scopes/aignostics-scopes.yml.\n  - flow: deviceCode\n    standard: RFC 8628\n    deviceAuthorizationUrl: https://aignostics-platform.eu.auth0.com/oauth/device/code\n    tokenUrl: https://aignostics-platform.eu.auth0.com/oauth/token\n    grant_type: urn:ietf:params:oauth:grant-type:device_code\n    audience: https://aignostics-platform-samia\n    scope:\
  \ offline_access\n    note: >-\n      Documented in the getting-started guide and supported by the tenant\n      (grant_types_supported includes the device-code URN) but NOT declared in the OpenAPI\n      securityScheme. A client generated from the spec alone will only know about the\n      authorization-code flow, even though device code is the flow the docs actually teach and the\n      one the SDK uses for headless and CLI callers.\n  sources:\n  - openapi/aignostics-platform-api-openapi.json\n  - https://aignostics.readthedocs.io/en/latest/get_started_api.html\ncredentials:\n  issuance: manual\n  detail: >-\n    A user account is created by organization invitation; the client_id is obtained from\n    support@aignostics.com. There is no client secret and no self-serve key generation. An\n    organization must be registered by the business support team before any of this is possible.\n  self_serve: false\n  rotation: not documented\ntokens:\n  access_token:\n    format: JWT\n    audience:\
  \ https://aignostics-platform-samia\n    lifetime: not published\n    validation: RS256 against the tenant JWKS\n  refresh_token:\n    issued_when: scope includes offline_access\n    use: >-\n      Renew the access token without a browser round trip - grant_type=refresh_token against\n      https://aignostics-platform.eu.auth0.com/oauth/token.\n  expiry_signal:\n    status: 401\n    body_observed: 'Jwt is missing'\n    note: >-\n      Observed live on 2026-09-14 at https://platform.aignostics.com/api/v1/applications - a\n      plain-text body, not JSON. The docs say treat 401 as \"renew and replay once\".\ndelegated_access:\n  mechanisms:\n  - name: grant\n    operation: create_grant_v1_access_grants_post\n    subjects: [user, organization_admin, organization_user, share_token]\n    relations_creatable: [viewer]\n    note: Only viewer grants may be created through the API; anything else returns 422.\n  - name: share token\n    operation: create_share_token_v1_access_share_tokens_post\n\
  \    parameter: share_token (query parameter on the run, item and artifact read operations)\n    secret_handling: >-\n      \"The returned share_token value is shown only once and is never stored.\"\n    expiry: caller-set expires_at at creation\n    revocation: >-\n      DELETE /v1/access/share-tokens/{share_token_id} \"invalidates the credential regardless of any\n      active grants\".\n    note: >-\n      This is the one credential in the system a machine can mint for another machine - and it is\n      well-shaped: single-display secret, caller-set expiry, independent revocation, and a\n      least-privilege default of viewer. It is scoped to sharing results, not to submitting work.\nsecondary_credentials:\n  warning: >-\n    GET /v1/me returns the organization's Google Cloud Storage HMAC access key ID AND secret access\n    key, a Logfire ingest token and a Sentry DSN inside the OrganizationReadResponse body. The\n    identity endpoint is therefore also a credential-distribution endpoint:\
  \ anything that logs,\n    caches or forwards a /v1/me response is handling live storage credentials. See\n    data-model/aignostics-data-model.yml.\n  source: openapi/aignostics-platform-api-openapi.json (OrganizationReadResponse field descriptions)\ngaps:\n- id: device-flow-undeclared-in-spec\n  detail: >-\n    The flow the documentation teaches is absent from the machine-readable contract. Adding a\n    deviceCode entry to the securityScheme flows would close the gap between the spec and the docs.\n- id: empty-scopes\n  detail: >-\n    The oauth2 scheme declares zero scopes, so the contract expresses no authorization granularity at\n    all - every token is, as far as a generated client can tell, all-or-nothing.\n- id: staging-urls-in-the-vendored-spec\n  detail: >-\n    The OpenAPI copy vendored in the SDK repo at docs/source/_static/openapi_v1.json (info.version\n    1.4.0) points its authorizationUrl and tokenUrl at\n    https://aignostics-platform-STAGING.eu.auth0.com. The live\
  \ document served at\n    https://platform.aignostics.com/api/v1/openapi.json (1.8.0) correctly points at the production\n    tenant. A developer generating a client from the repo copy - which the README links as the\n    OpenAPI specification - gets a client that authenticates against staging.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aignostics/refs/heads/main/authentication/aignostics-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine-Learning
- Health
- Healthcare
- Life Sciences
- Pathology
- Medical Imaging
- Digital Pathology
- Oncology
- Biotechnology
- Research
- Germany
---
