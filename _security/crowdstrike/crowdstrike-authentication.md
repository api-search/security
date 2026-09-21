---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: Every CrowdStrike Falcon API call is authenticated with an OAuth2 client-credentials bearer token. API clients (client_id + client_secret) are created inside the Falcon console under Support and resources > API Clients & Keys and are scoped at creation time; there is no anonymous, self-serve or delegated-user flow. Derived from the provider's own OAuth2 service-collection reference rather than an OpenAPI document — CrowdStrike publishes no spec.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crowdstrike Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: CrowdStrike secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: CrowdStrike
provider_slug: crowdstrike
scheme_count: 1
schemes:
- error_statuses:
  - 400
  - 403
  - 429
  - 500
  flow: clientCredentials
  name: FalconOAuth2
  operations:
    issue: oauth2AccessToken
    revoke: oauth2RevokeToken
  presentation: 'Authorization: Bearer <access_token>'
  request:
    content_type: application/x-www-form-urlencoded
    method: POST
    parameters:
    - in: body
      name: client_id
      required: true
    - in: body
      name: client_secret
      required: true
    - description: MSSP master CIDs may lock the token to act on behalf of a member CID
      in: body
      name: member_cid
      required: false
    - in: body
      name: alter_state
      required: false
  response:
    fields:
    - access_token
    - expires_in
    - id_token
    - issued_token_type
    - refresh_token
    - scope
    - token_type
    status: 201
  revoke_url: https://api.crowdstrike.com/oauth2/revoke
  sources:
  - https://developer.crowdstrike.com/api-reference/collections/oauth2/
  - https://developer.crowdstrike.com/llms.txt
  token_lifetime: 30 minutes (documented); revoke early with oauth2RevokeToken
  token_url: https://api.crowdstrike.com/oauth2/token
  type: oauth2
slug: crowdstrike-authentication
source_filename: crowdstrike-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: CrowdStrike\nproviderId: crowdstrike\ngenerated: '2026-09-19'\nmethod: searched\nsource: https://developer.crowdstrike.com/api-reference/collections/oauth2/\ndocs: https://developer.crowdstrike.com/falcon-mcp/getting-started/credentials/\ndescription: Every CrowdStrike Falcon API call is authenticated with an OAuth2 client-credentials bearer token.\n  API clients (client_id + client_secret) are created inside the Falcon console under Support and resources > API\n  Clients & Keys and are scoped at creation time; there is no anonymous, self-serve or delegated-user flow. Derived\n  from the provider's own OAuth2 service-collection reference rather than an OpenAPI document — CrowdStrike publishes\n  no spec.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n  oauth2_flows:\n  - clientCredentials\n  openid_connect: false\n  mutual_tls: false\n  note: An `id_token` field is present in the token response\
  \ body, but no OIDC discovery document is served on any\n    CrowdStrike host (see well-known/crowdstrike-well-known.yml).\nschemes:\n- name: FalconOAuth2\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.crowdstrike.com/oauth2/token\n  revoke_url: https://api.crowdstrike.com/oauth2/revoke\n  operations:\n    issue: oauth2AccessToken\n    revoke: oauth2RevokeToken\n  request:\n    method: POST\n    content_type: application/x-www-form-urlencoded\n    parameters:\n    - name: client_id\n      in: body\n      required: true\n    - name: client_secret\n      in: body\n      required: true\n    - name: member_cid\n      in: body\n      required: false\n      description: MSSP master CIDs may lock the token to act on behalf of a member CID\n    - name: alter_state\n      in: body\n      required: false\n  response:\n    status: 201\n    fields:\n    - access_token\n    - expires_in\n    - id_token\n    - issued_token_type\n    - refresh_token\n    - scope\n    - token_type\n\
  \  presentation: 'Authorization: Bearer <access_token>'\n  token_lifetime: 30 minutes (documented); revoke early with oauth2RevokeToken\n  error_statuses:\n  - 400\n  - 403\n  - 429\n  - 500\n  sources:\n  - https://developer.crowdstrike.com/api-reference/collections/oauth2/\n  - https://developer.crowdstrike.com/llms.txt\nregions:\n- cloud: us-1\n  base_url: https://api.crowdstrike.com\n  default: true\n- cloud: us-2\n  base_url: https://api.us-2.crowdstrike.com\n- cloud: eu-1\n  base_url: https://api.eu-1.crowdstrike.com\n- cloud: us-gov-1\n  base_url: https://api.laggar.gcw.crowdstrike.com\nauthorization:\n  model: scope-per-service-collection\n  detail: 'Each API client is granted a set of named scopes of the form ''<Service>: READ'' or ''<Service>: WRITE''.\n    Every operation in the reference states the scope it requires. See scopes/crowdstrike-scopes.yml (187 scopes).'\n  console_path: Support and resources > API Clients & Keys\nx-evidence:\n  probed: '2026-09-19'\n  url: https://api.crowdstrike.com/oauth2/token\n\
  \  http_status: 401\n  note: Unauthenticated POST returns 401 with the Falcon error envelope and X-Cs-Traceid / X-Ratelimit-* headers\n    — the auth surface is live and rejects anonymous callers.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdstrike/refs/heads/main/authentication/crowdstrike-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Cybersecurity
- Endpoint Security
- EDR
- Threat Intelligence
- Cloud Security
- Identity Protection
- Vulnerability Management
- SIEM
- Security Operations
- MCP
---
