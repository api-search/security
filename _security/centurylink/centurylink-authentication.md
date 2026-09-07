---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Centurylink Authentication
name_suffix: Authentication
oauth_flows: []
overview: CenturyLink (Lumen Technologies) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: CenturyLink (Lumen Technologies)
provider_slug: centurylink
scheme_count: 3
schemes:
- credential_transport: HTTP Basic (consumer key as username, consumer secret as password)
  description: Lumen API products use OAuth 2.0 client credentials. The consumer key and consumer secret issued against an API key in Lumen Connect are sent as HTTP Basic credentials to the Lumen authorization server; the returned access token is then presented as a Bearer token on each API call.
  flow: clientCredentials
  id: oauth2_client_credentials
  token_endpoints:
  - http_status_unauthenticated: 401
    method: probed
    note: Legacy token endpoint. A GET returns 500 with {"ErrorCode":"invalid_grant_type","Error":"grant_type is required"}; a POST with grant_type=client_credentials and no credentials returns 401. Responses carry a TrackingId correlation header and Access-Control-Allow-Origin *.
    observed: '2026-09-05'
    observed_body: '{"ErrorCode":"invalid_client","Error":"Client identifier is required"}'
    url: https://api.lumen.com/oauth/v1/token
  - http_status_unauthenticated: 401
    method: probed
    note: Current token endpoint. The error body identifies an Apigee gateway and uses a code/reason/message/referenceError envelope.
    observed: '2026-09-05'
    observed_body: '{"reason":"Missing or no credentials provided","message":"000 -- ME-apigee...","referenceError":"","code":"missingCredentials"}'
    url: https://api.lumen.com/oauth/v2/token
  token_transport: Authorization Bearer
  type: oauth2
- description: API keys are created and managed in the Lumen Connect portal. Each key is scoped to the API products it covers, can be edited to change that product coverage, and its client secret can be reset independently of the key. Registration for API access is a prerequisite and is administrator-gated.
  id: api_key_registration
  management_docs:
  - https://docs.lumen.com/lumen-connect/apis/registering-for-api-access/
  - https://docs.lumen.com/lumen-connect/apis/creating-an-api-key/
  - https://docs.lumen.com/lumen-connect/apis/editing-an-api-key/
  - https://docs.lumen.com/lumen-connect/apis/deleting-an-api-key/
  - https://docs.lumen.com/lumen-connect/apis/resetting-the-client-secret-for-an-api-key/
  type: apiKey
- description: Lumen Edge Private Cloud uses its own API authentication token, created and managed inside the Edge Private Cloud product rather than through Lumen Connect API keys.
  id: edge_private_cloud_token
  management_docs:
  - https://docs.lumen.com/edge-private-cloud/creating-an-api-authentication-token-for-edge-private-cloud/
  - https://docs.lumen.com/edge-private-cloud/managing-api-sessions-for-edge-private-cloud/
  type: apiKey
slug: centurylink-authentication
source_filename: centurylink-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: CenturyLink (Lumen Technologies)\nproviderId: centurylink\ngenerated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://docs.lumen.com/lumen-connect/apis/ (server-rendered first-party documentation)\n  plus live anonymous probes of the Lumen API gateway at https://api.lumen.com\nnote: >-\n  Derived from documentation plus live probes, NOT from an OpenAPI document. Lumen\n  publishes no anonymously reachable machine-readable contract: the Developer Center\n  at developer.lumen.com is a Vue module-federation SPA that returns an identical\n  11,800-byte HTML shell for every path, and its OpenAPI specs are fetched at runtime\n  from a sign-in-gated content service.\nprimary_scheme: oauth2\nschemes:\n  - id: oauth2_client_credentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Lumen API products use OAuth 2.0 client credentials. The consumer key and consumer\n   \
  \   secret issued against an API key in Lumen Connect are sent as HTTP Basic credentials\n      to the Lumen authorization server; the returned access token is then presented as a\n      Bearer token on each API call.\n    token_endpoints:\n      - url: https://api.lumen.com/oauth/v1/token\n        method: probed\n        observed: '2026-09-05'\n        http_status_unauthenticated: 401\n        observed_body: '{\"ErrorCode\":\"invalid_client\",\"Error\":\"Client identifier is required\"}'\n        note: >-\n          Legacy token endpoint. A GET returns 500 with\n          {\"ErrorCode\":\"invalid_grant_type\",\"Error\":\"grant_type is required\"}; a POST with\n          grant_type=client_credentials and no credentials returns 401. Responses carry a\n          TrackingId correlation header and Access-Control-Allow-Origin *.\n      - url: https://api.lumen.com/oauth/v2/token\n        method: probed\n        observed: '2026-09-05'\n        http_status_unauthenticated: 401\n        observed_body:\
  \ '{\"reason\":\"Missing or no credentials provided\",\"message\":\"000 -- ME-apigee...\",\"referenceError\":\"\",\"code\":\"missingCredentials\"}'\n        note: >-\n          Current token endpoint. The error body identifies an Apigee gateway and uses a\n          code/reason/message/referenceError envelope.\n    token_transport: Authorization Bearer\n    credential_transport: 'HTTP Basic (consumer key as username, consumer secret as password)'\n  - id: api_key_registration\n    type: apiKey\n    description: >-\n      API keys are created and managed in the Lumen Connect portal. Each key is scoped to\n      the API products it covers, can be edited to change that product coverage, and its\n      client secret can be reset independently of the key. Registration for API access is\n      a prerequisite and is administrator-gated.\n    management_docs:\n      - https://docs.lumen.com/lumen-connect/apis/registering-for-api-access/\n      - https://docs.lumen.com/lumen-connect/apis/creating-an-api-key/\n\
  \      - https://docs.lumen.com/lumen-connect/apis/editing-an-api-key/\n      - https://docs.lumen.com/lumen-connect/apis/deleting-an-api-key/\n      - https://docs.lumen.com/lumen-connect/apis/resetting-the-client-secret-for-an-api-key/\n  - id: edge_private_cloud_token\n    type: apiKey\n    description: >-\n      Lumen Edge Private Cloud uses its own API authentication token, created and managed\n      inside the Edge Private Cloud product rather than through Lumen Connect API keys.\n    management_docs:\n      - https://docs.lumen.com/edge-private-cloud/creating-an-api-authentication-token-for-edge-private-cloud/\n      - https://docs.lumen.com/edge-private-cloud/managing-api-sessions-for-edge-private-cloud/\nonboarding:\n  self_service: false\n  requires_contract: true\n  description: >-\n    API access is not self-service. A Lumen Connect account is required, the account must\n    be registered for API access, and an administrator must enable the API products a key\n    covers. There\
  \ is no anonymous key issuance and no public trial credential.\ndocs:\n  - https://docs.lumen.com/lumen-connect/apis/\n  - https://developer.lumen.com/devcenter/getting-started\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centurylink/refs/heads/main/authentication/centurylink-authentication.yml
summary_line: 3 schemes
tags:
- Broadband
- Connectivity
- Edge
- Fiber
- Lumen
- Network
- Authentication
- Quantum Fiber
- SD-WAN
- Telecom
- Fortune 500
---
