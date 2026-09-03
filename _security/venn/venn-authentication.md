---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Venn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Venn declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Venn
provider_slug: venn
scheme_count: 0
schemes: []
slug: venn-authentication
source_filename: venn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://api.venn.city/production/graphql\nnote: >-\n  Venn publishes no developer authentication guide. This profile is assembled from\n  three public, unauthenticated sources: (1) live behaviour of the Venn tenant\n  GraphQL gateway at https://api.venn.city/production/graphql, (2) the OpenID\n  Connect discovery document of the AWS Cognito user pool that Venn's own operator\n  dashboard bundle names as its identity provider, and (3) the public README of\n  Venn's first-party `@venncity/extension-sdk` npm package, which documents how a\n  resident token reaches an embedded app. No credentials were used and no access\n  control was defeated.\napis:\n  - name: Venn Tenant GraphQL API\n    base_url: https://api.venn.city/production/graphql\n    transport: https\n    schemes:\n      - id: bearer-jwt\n        type: http\n        scheme: bearer\n        bearer_format: JWT\n        in: header\n        header: Authorization\n       \
  \ value: 'Bearer <cognito-access-token>'\n        issuer: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx\n        jwks_uri: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx/.well-known/jwks.json\n        signing_alg: RS256\n        evidence: >-\n          The gateway advertises `Authorization` in its\n          Access-Control-Allow-Headers on every response; the extension SDK README\n          states the bridge delivers \"the resident's existing Cognito token\" and\n          that \"the Venn tenant GraphQL API is the authority that validates it (a\n          401 means 'ask the host for a fresh one')\".\n        required: true\n      - id: api-key\n        type: apiKey\n        in: header\n        header: X-Api-Key\n        evidence: >-\n          `X-Api-Key` is advertised in the gateway's Access-Control-Allow-Headers,\n          and the schema exposes a first-class `UserApiKey` entity with\n          `userApiKey`/`userApiKeys` queries and\n \
  \         `createUserApiKey`/`updateUserApiKey`/`deleteUserApiKey` mutations — so\n          per-user API keys are a modelled, self-service credential. No public\n          documentation describes how to obtain or scope one.\n        required: false\n        documented_publicly: false\n      - id: aws-sigv4\n        type: http\n        scheme: aws-sigv4\n        evidence: >-\n          `X-Amz-Date`, `X-Amz-Security-Token` and `X-Amz-User-Agent` are advertised\n          in Access-Control-Allow-Headers, which is the AWS Amplify/API Gateway\n          default set. Present at the edge; not observed to be the primary\n          credential.\n        required: false\nidentity_provider:\n  vendor: AWS Cognito\n  region: eu-central-1\n  user_pool: eu-central-1_cH7XNjcIx\n  domain: https://admin-tool.auth.eu-central-1.amazoncognito.com\n  discovery: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx/.well-known/openid-configuration\n  discovery_status: 200\n  document: ../well-known/venn-openid-configuration.json\n\
  \  protocols:\n    - openid-connect\n    - oauth2\n  flows:\n    - authorization_code\n    - implicit\n  response_types: [code, token]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post]\n  revocation_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/oauth2/revoke\n  end_session_endpoint: https://admin-tool.auth.eu-central-1.amazoncognito.com/logout\n  note: >-\n    This pool serves Venn's operator/admin tooling. Resident-facing sign-in in the\n    mobile app issues a Cognito token of the same family (per the extension SDK\n    README, which hands the guest both a `token` and a `refreshToken` and tells it\n    to refresh \"yourself against Cognito\"). Whether residents and operators share\n    this pool could not be established from public sources.\nauthorization:\n  model: role-based, tenant-scoped\n  evidence: >-\n    The schema exposes `Role` / `roles` / `createRole` and per-community\n    (`hood`), per-building and per-portfolio settings entities;\
  \ errors from the\n    persistency service on unauthenticated reads are tenant-authorization failures,\n    not schema failures.\n  scopes_document: ../scopes/venn-scopes.yml\nobserved_behaviour:\n  - probe: 'POST /production/graphql  {__schema{queryType{name}}}  (no credentials)'\n    status: 200\n    result: >-\n      Full introspection succeeded anonymously — 1,991 types, 320 query fields,\n      357 mutation fields. The CONTRACT is public.\n  - probe: 'POST /production/graphql  {users(first:1){id}}  (no credentials)'\n    status: 200\n    result: >-\n      GraphQL error `VennUnknownError` from serviceName `persistency`, data null.\n      The DATA is gated. Introspection being open does not imply readable data.\n  - probe: 'GET https://api.venn.city/  and every non-stage path'\n    status: 403\n    result: AWS API Gateway ForbiddenException; only the `/production/` stage is routable.\nmfa:\n  supported: true\n  evidence: >-\n    `@venncity/extension-sdk` exposes `invokeElevatedPermissions(reason)`\
  \ for a\n    step-up 2FA prompt, documented in its README as \"stubbed today\".\n  status: partial\ngaps:\n  - No public authentication documentation, quickstart or key-issuance flow.\n  - No documented way for a third party to obtain credentials; access appears to follow a customer contract.\n  - Anonymous GraphQL introspection is enabled on the production gateway. Venn may or may not intend this.\nx-evidence:\n  checked: '2026-09-02'\n  evidence:\n    - url: https://api.venn.city/production/graphql\n      status: 200\n    - url: https://cognito-idp.eu-central-1.amazonaws.com/eu-central-1_cH7XNjcIx/.well-known/openid-configuration\n      status: 200\n    - url: https://registry.npmjs.org/@venncity%2Fextension-sdk\n      status: 200\n    - url: https://www.npmjs.com/package/@venncity/extension-sdk\n      status: 403\n      note: npmjs.com web UI refuses non-browser user agents; the registry API above returned the same package metadata and README.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/venn/refs/heads/main/authentication/venn-authentication.yml
summary_line: 0 schemes
tags:
- Real Estate
- Property Management
- Multifamily
- Resident Experience
- Proptech
- Leasing
- Community
- Payments
- GraphQL
- Mobile Apps
---
