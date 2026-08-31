---
api_key_in: []
auth_types: []
description: 'Authentication profile for the Blameless API, reconstructed from Blameless'' own published client code and from its still-live Auth0 identity tenant. Blameless published no OpenAPI, and its documentation host (docs.blameless.com) no longer resolves, so nothing here is derived from a spec — every scheme below is grounded in a fetched first-party artifact. The API itself is retired: the tenant hosts these credentials were presented to (<instance>.blameless.io) no longer exist in DNS.'
kind: authentication
layout: security
method: probed
name: Blameless Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blameless declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Blameless
provider_slug: blameless
scheme_count: 3
schemes:
- audience: <instance_name>.blameless.io
  credential_issuance: manual
  credential_issuance_note: Not self-service. The SLO CLI README instructs users to contact Blameless Customer Success (cs@blameless.io) to be issued a client id and secret bound to their instance.
  evidence:
  - https://github.com/blamelesshq/blameless-openslo/blob/main/src/lib/config/env.js
  - https://github.com/blamelesshq/blameless-openslo#initial-setup
  - https://blamelesshq.auth0.com/.well-known/openid-configuration
  flow: clientCredentials
  grant_type: client_credentials
  id: oauth2_client_credentials
  issuer: https://blamelesshq.auth0.com/
  jwks_uri: https://blamelesshq.auth0.com/.well-known/jwks.json
  label: Auth0 machine-to-machine client credentials
  parameters:
  - name: BLAMELESS_OAUTH_CLIENT_ID
  - name: BLAMELESS_OAUTH_CLIENT_SECRET
  - name: BLAMELESS_OAUTH_AUDIENCE
  token_endpoint: https://blamelesshq.auth0.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  type: oauth2
- description: Every call to the tenant API carried the Auth0 access token as an Authorization bearer header. Blameless' Go sample client sets the auth scheme to Bearer explicitly; the Node client sets the Authorization header in an axios request interceptor and retries once on 401.
  evidence:
  - https://github.com/blamelesshq/blameless-api-samples/blob/main/go/slo/packages/clients/blameless.go
  - https://github.com/blamelesshq/blameless-openslo/blob/main/src/blameless-delete/handlers/shared/apiCall.js
  header: 'Authorization: Bearer <token>'
  id: bearer_token
  label: Bearer access token on the tenant API
  scheme: bearer
  type: http
- description: The Terraform provider authenticates with an instance URL plus an API key, sourced from BLAMELESS_INSTANCE and BLAMELESS_KEY. The provider documentation does not state which header carries the key, and the provider source is the only reference.
  evidence:
  - https://github.com/blamelesshq/terraform-provider-blameless/blob/main/docs/index.md
  id: api_key
  in: header
  label: Blameless API key (Terraform provider)
  parameters:
  - name: BLAMELESS_INSTANCE
  - name: BLAMELESS_KEY
  type: apiKey
slug: blameless-authentication
source_filename: blameless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://blamelesshq.auth0.com/.well-known/openid-configuration (200, 2026-08-29) + https://github.com/blamelesshq/blameless-openslo/blob/main/src/lib/config/env.js + https://github.com/blamelesshq/terraform-provider-blameless/blob/main/docs/index.md\nspecification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Blameless\nproviderId: blameless\nstatus: historical\ndescription: >-\n  Authentication profile for the Blameless API, reconstructed from Blameless' own published\n  client code and from its still-live Auth0 identity tenant. Blameless published no OpenAPI,\n  and its documentation host (docs.blameless.com) no longer resolves, so nothing here is\n  derived from a spec — every scheme below is grounded in a fetched first-party artifact.\n  The API itself is retired: the tenant hosts these credentials were presented to\n  (<instance>.blameless.io) no longer exist in DNS.\nschemes:\n  - id: oauth2_client_credentials\n\
  \    type: oauth2\n    flow: clientCredentials\n    label: Auth0 machine-to-machine client credentials\n    token_endpoint: https://blamelesshq.auth0.com/oauth/token\n    issuer: https://blamelesshq.auth0.com/\n    jwks_uri: https://blamelesshq.auth0.com/.well-known/jwks.json\n    grant_type: client_credentials\n    audience: <instance_name>.blameless.io\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - none\n    parameters:\n      - name: BLAMELESS_OAUTH_CLIENT_ID\n      - name: BLAMELESS_OAUTH_CLIENT_SECRET\n      - name: BLAMELESS_OAUTH_AUDIENCE\n    credential_issuance: manual\n    credential_issuance_note: >-\n      Not self-service. The SLO CLI README instructs users to contact Blameless Customer\n      Success (cs@blameless.io) to be issued a client id and secret bound to their instance.\n    evidence:\n      - https://github.com/blamelesshq/blameless-openslo/blob/main/src/lib/config/env.js\n      - https://github.com/blamelesshq/blameless-openslo#initial-setup\n\
  \      - https://blamelesshq.auth0.com/.well-known/openid-configuration\n  - id: bearer_token\n    type: http\n    scheme: bearer\n    label: Bearer access token on the tenant API\n    header: 'Authorization: Bearer <token>'\n    description: >-\n      Every call to the tenant API carried the Auth0 access token as an Authorization\n      bearer header. Blameless' Go sample client sets the auth scheme to Bearer explicitly;\n      the Node client sets the Authorization header in an axios request interceptor and\n      retries once on 401.\n    evidence:\n      - https://github.com/blamelesshq/blameless-api-samples/blob/main/go/slo/packages/clients/blameless.go\n      - https://github.com/blamelesshq/blameless-openslo/blob/main/src/blameless-delete/handlers/shared/apiCall.js\n  - id: api_key\n    type: apiKey\n    in: header\n    label: Blameless API key (Terraform provider)\n    description: >-\n      The Terraform provider authenticates with an instance URL plus an API key, sourced\n  \
  \    from BLAMELESS_INSTANCE and BLAMELESS_KEY. The provider documentation does not state\n      which header carries the key, and the provider source is the only reference.\n    parameters:\n      - name: BLAMELESS_INSTANCE\n      - name: BLAMELESS_KEY\n    evidence:\n      - https://github.com/blamelesshq/terraform-provider-blameless/blob/main/docs/index.md\nauthorization:\n  model: rule-based\n  note: >-\n    The removed reference documented an \"API Access Control\" model in which each operation\n    required a named rule — GET /api/v1/incidents required IncidentRead. Recorded at low\n    confidence: the page (docs.blameless.com/features/api-access-control/) is only present\n    in search-engine memory and returns nothing today, since the host has no DNS record.\n  confidence: low\n  evidence:\n    - url: https://docs.blameless.com/features/api-access-control/\n      status: 0\n      note: NXDOMAIN 2026-08-29.\ngaps:\n  - >-\n    A documented workaround in the CLI how-to told users\
  \ to copy an access_token out of the\n    web UI into BLAMELESS_TEMP_AUTH_TOKEN because of a \"known login issue\" — a\n    provider-acknowledged break in the machine credential path.\n  - >-\n    No refresh-token handling: the Node client's 401 interceptor contains a TODO noting the\n    token-refresh API did not exist yet.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blameless/refs/heads/main/authentication/blameless-authentication.yml
summary_line: 3 schemes
tags:
- AIOps
- SRE
- Incident Management
- Reliability
- Service Level Objectives
- Retrospectives
- On-Call
- DevOps
---
