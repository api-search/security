---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fusebit-accounts-api-openapi.yml
  format: yaml
  label: Fusebit Accounts API
  slug: fusebit-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-accounts-api-openapi.yml
- filename: fusebit-boundaries-api-openapi.yml
  format: yaml
  label: Fusebit Boundaries API
  slug: fusebit-boundaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-boundaries-api-openapi.yml
- filename: fusebit-clients-api-openapi.yml
  format: yaml
  label: Fusebit Clients API
  slug: fusebit-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-clients-api-openapi.yml
- filename: fusebit-connector-api-openapi.yml
  format: yaml
  label: Fusebit Connector API
  slug: fusebit-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-connector-api-openapi.yml
- filename: fusebit-connector-tags-api-openapi.yml
  format: yaml
  label: Fusebit Connector/Tags API
  slug: fusebit-connector-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-connector-tags-api-openapi.yml
- filename: fusebit-functions-api-openapi.yml
  format: yaml
  label: Fusebit Functions API
  slug: fusebit-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-functions-api-openapi.yml
- filename: fusebit-identity-api-openapi.yml
  format: yaml
  label: Fusebit Identity API
  slug: fusebit-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-identity-api-openapi.yml
- filename: fusebit-identity-tags-api-openapi.yml
  format: yaml
  label: Fusebit Identity/Tags API
  slug: fusebit-identity-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-identity-tags-api-openapi.yml
- filename: fusebit-install-api-openapi.yml
  format: yaml
  label: Fusebit Install API
  slug: fusebit-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-install-api-openapi.yml
- filename: fusebit-install-tags-api-openapi.yml
  format: yaml
  label: Fusebit Install/Tags API
  slug: fusebit-install-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-install-tags-api-openapi.yml
- filename: fusebit-integration-api-openapi.yml
  format: yaml
  label: Fusebit Integration API
  slug: fusebit-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-integration-api-openapi.yml
- filename: fusebit-integration-tags-api-openapi.yml
  format: yaml
  label: Fusebit Integration/Tags API
  slug: fusebit-integration-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-integration-tags-api-openapi.yml
- filename: fusebit-issuers-api-openapi.yml
  format: yaml
  label: Fusebit Issuers API
  slug: fusebit-issuers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-issuers-api-openapi.yml
- filename: fusebit-registry-api-openapi.yml
  format: yaml
  label: Fusebit Registry API
  slug: fusebit-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-registry-api-openapi.yml
- filename: fusebit-session-api-openapi.yml
  format: yaml
  label: Fusebit Session API
  slug: fusebit-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-session-api-openapi.yml
- filename: fusebit-storage-api-openapi.yml
  format: yaml
  label: Fusebit Storage API
  slug: fusebit-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-storage-api-openapi.yml
- filename: fusebit-subscriptions-api-openapi.yml
  format: yaml
  label: Fusebit Subscriptions API
  slug: fusebit-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-subscriptions-api-openapi.yml
- filename: fusebit-users-api-openapi.yml
  format: yaml
  label: Fusebit Users API
  slug: fusebit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/openapi/fusebit-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fusebit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fusebit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fusebit
provider_slug: fusebit
scheme_count: 1
schemes:
- applied: global
  bearerFormat: JWT
  description: 'The only securityScheme in either contract, applied globally at the document root of both v1 and v2. Presented as `Authorization: Bearer <jwt>`.'
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/fusebit-http-api-core-openapi.yml
  - openapi/fusebit-http-api-integrations-openapi.yml
  type: http
slug: fusebit-authentication
source_filename: fusebit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: derived\nsource: >-\n  openapi/fusebit-http-api-core-openapi.yml, openapi/fusebit-http-api-integrations-openapi.yml.\n  The narrative auth pages both specs link to (developer.fusebit.io/docs/connecting-fusebit-with-your-\n  application and fusebit.io/docs/integrator-guide/authz-model) were probed on 2026-09-10 and fail DNS\n  resolution, so this profile is grounded entirely in the contracts and the CLI command tree.\nprovider: Fusebit\nproviderId: fusebit\nsummary:\n  types:\n    - http\n  models:\n    - bearer-jwt\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\nschemes:\n  - name: AccessToken\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applied: global\n    description: >-\n      The only securityScheme in either contract, applied globally at the document root of both v1\n      and v2. Presented as `Authorization: Bearer <jwt>`.\n    sources:\n      - openapi/fusebit-http-api-core-openapi.yml\n      - openapi/fusebit-http-api-integrations-openapi.yml\n\
  token_issuance:\n  model: trusted-issuer\n  description: >-\n    Fusebit does not mint tokens from a Fusebit-operated authorization server. An account registers\n    one or more trusted JWT ISSUERS (postAccountIssuer), each carrying either inline public keys or a\n    jsonKeysUrl. Any JWT signed by a registered issuer and matching a registered Identity is accepted.\n  entities:\n    - name: Issuer\n      operations: [getAccountIssuerList, getAccountIssuer, postAccountIssuer, putAccountIssuer, deleteIssuer]\n      fields: [displayName, jsonKeysUrl, 'publicKeys[] { keyId, publicKey }']\n    - name: Identity\n      shape: '{ issuerId, subject }'\n      description: >-\n        Binds the `iss` and `sub` claims of an incoming token to a Fusebit User or Client. A principal\n        may hold several identities.\n  bootstrap:\n    mechanism: init token\n    operations: [initUser, initClient, resolveInit]\n    description: >-\n      A new principal is onboarded with a one-time init token, redeemed\
  \ through resolveInit (or\n      `fuse init <token>` in the CLI), which provisions the local profile and its keypair. This is how\n      Fusebit avoided shipping a password or API-key surface at all.\nauthorization:\n  model: action-and-resource\n  is_oauth_scopes: false\n  shape: 'AccessStatement { action, resource }'\n  description: >-\n    Authorization is an explicit allow-list attached to the User or Client. `action` is a\n    colon-delimited verb, optionally wildcarded (\"function:*\"); `resource` is a hierarchical path such\n    as /account/{accountId}/subscription/{subscriptionId}/boundary/{boundaryId}/function/{functionId},\n    and a grant on a prefix implies everything beneath it. Because this is a grant list rather than an\n    OAuth scope set, no scopes/ artifact is emitted for Fusebit.\n  managed_by:\n    cli: ['fuse user access add', 'fuse user access rm', 'fuse client access add', 'fuse client access rm']\n    api: [postUser, patchUser, postClient, putAccountClient]\n \
  \ actions:\n    - action: account:get\n      description: Read the account.\n    - action: account:patch\n      description: Update the account.\n    - action: audit:get\n      description: Read the account audit trail.\n    - action: subscription:get\n      description: Read a subscription.\n    - action: user:add\n      description: Create a user.\n    - action: user:get\n      description: Read a user.\n    - action: user:update\n      description: Update a user, including its access grants and identities.\n    - action: user:delete\n      description: Delete a user.\n    - action: user:init\n      description: Issue an init token for a user.\n    - action: client:add\n      description: Create a machine client.\n    - action: client:get\n      description: Read a client.\n    - action: client:update\n      description: Update a client.\n    - action: client:delete\n      description: Delete a client.\n    - action: client:init\n      description: Issue an init token for a client.\n\
  \    - action: issuer:add\n      description: Register a trusted JWT issuer.\n    - action: issuer:get\n      description: Read an issuer.\n    - action: issuer:update\n      description: Update an issuer or its public keys.\n    - action: issuer:delete\n      description: Remove a trusted issuer.\n    - action: function:get\n      description: Read a function.\n    - action: function:put\n      description: Create or update a function.\n    - action: function:delete\n      description: Delete a function.\n    - action: function:get-log\n      description: Read a function's execution logs.\n    - action: function:schedule\n      description: Schedule an execution on a function task route.\n    - action: log:get\n      description: Read logs at account, subscription, boundary or function scope.\n    - action: storage:get\n      description: Read subscription-scoped storage.\n    - action: storage:put\n      description: Write subscription-scoped storage.\n    - action: storage:delete\n\
  \      description: Delete subscription-scoped storage.\n    - action: registry:get\n      description: Read the account's private npm registry configuration.\n    - action: integration:add\n      description: Create an integration (v2).\n    - action: integration:get\n      description: Read an integration (v2).\n    - action: integration:put\n      description: Replace an integration (v2).\n    - action: integration:update\n      description: Update an integration (v2).\n    - action: integration:delete\n      description: Delete an integration (v2).\n    - action: integration:put-tag\n      description: Set or remove an integration tag (v2).\n    - action: connector:add\n      description: Create a connector (v2).\n    - action: connector:get\n      description: Read a connector (v2).\n    - action: connector:update\n      description: Update a connector (v2).\n    - action: connector:delete\n      description: Delete a connector (v2).\n    - action: connector:put-tag\n      description:\
  \ Set or remove a connector tag (v2).\n    - action: identity:get\n      description: Read a managed third-party credential (v2).\n    - action: identity:update\n      description: Update a managed third-party credential (v2).\n    - action: identity:delete\n      description: Delete a managed third-party credential (v2).\n    - action: identity:put-tag\n      description: Set or remove an identity tag (v2).\n    - action: install:get\n      description: Read an install (v2).\n    - action: install:put-tag\n      description: Set or remove an install tag (v2).\n    - action: instance:get\n      description: Read an install instance (v2, legacy naming).\n    - action: instance:update\n      description: Update an install instance (v2, legacy naming).\n    - action: instance:delete\n      description: Delete an install instance (v2, legacy naming).\nchallenge_semantics:\n  unauthenticated_status: 403\n  www_authenticate: false\n  note: >-\n    Neither contract declares a 401 response or\
  \ a WWW-Authenticate challenge header on any operation.\n    A missing, expired or insufficiently-granted token is answered 403 in all three cases, so a client\n    cannot distinguish \"not authenticated\" from \"not authorized\" from the status code alone.\nthird_party_oauth:\n  note: >-\n    Distinct from Fusebit's OWN auth: Fusebit's product was managing OAuth 2.0 credentials for OTHER\n    services on behalf of its customers. 40 of its 80 @fusebit-int packages are OAuth connectors\n    (Slack, Salesforce, HubSpot, Xero, Atlassian, QuickBooks, Google, Microsoft Graph and more), plus a\n    generic oauth-connector, a client-credentials-flow connector and a private-key connector. Those\n    flows are the CONSUMING side and are catalogued in packages/fusebit-packages.yml, not here.\ncallable: false\ncallable_note: >-\n  Historical profile. api.us-west-1.on.fusebit.io returns NXDOMAIN (2026-09-10); no token can be\n  presented to anything.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusebit/refs/heads/main/authentication/fusebit-authentication.yml
summary_line: http · 1 scheme
tags:
- Developer Tools
- Embedded iPaaS
- Integration
- Serverless
- Authentication
- Acquired
- Defunct
---
