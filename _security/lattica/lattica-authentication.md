---
api_key_in: []
auth_types: []
description: 'Lattica does not publish an OpenAPI definition, so this profile was read off the platform documentation and the official Python SDK rather than derived from securitySchemes. There is no OAuth 2.0 and no OpenID Connect: the whole platform authenticates with bearer tokens, but with TWO distinct token classes that are easy to conflate — an organization-level management license and a per-user, per-workload query token.'
kind: authentication
layout: security
method: searched
name: Lattica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lattica declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lattica
provider_slug: lattica
scheme_count: 2
schemes:
- audience: Organization administrator
  docs: https://platformdocs.lattica.ai/how-to-guides/access-control/how-to-create-user-access-token.md
  expiration: Not documented.
  format: 'Authorization: Bearer <token>'
  grants: Full management surface — create/activate/deactivate workloads (models), generate and assign user access tokens, start/stop compute workers, read account info, credits, and transaction history.
  header: Authorization
  id: management_license
  in: header
  issued_by: Lattica web console (https://console.lattica.ai/)
  rotation: Not documented.
  scheme: bearer
  sdk_usage: LatticaManagement("your_license_from_lattica_console")
  type: http
- audience: End user querying a workload
  docs: https://platformdocs.lattica.ai/architecture-overview/query-client.md
  expiration: 30 days — tokens must be renewed on expiry.
  format: 'Authorization: Bearer <token>'
  grants: Submit encrypted queries to the assigned workload, upload an evaluation key, and retrieve the encrypted result. No management capability.
  header: Authorization
  id: user_access_token
  in: header
  issued_by: The workload service provider, via the web console (Token Management) or the Python management SDK (generate_query_token).
  retrievability: Shown once at creation and NOT stored by the platform. It cannot be retrieved later; a lost token must be replaced.
  revocation: Tokens can be updated, reassigned, deleted, or set active/cancelled from the console or the management SDK (update_token_info, assign_token_to_model, unassign_token_from_model, delete_token).
  scheme: bearer
  scoping: Bound to ONE user and ONE workload. A token may be created unassigned and linked to a workload later; an end user cannot use an unassigned token.
  token_format: JWT
  type: http
slug: lattica-authentication
source_filename: lattica-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://platformdocs.lattica.ai/architecture-overview/query-client.md,\n  https://platformdocs.lattica.ai/how-to-guides/access-control/how-to-create-user-access-token.md,\n  https://platformdocs.lattica.ai/how-to-guides/secure-query-processing/how-to-execute-query.md;\n  transport detail confirmed in the first-party lattica-common 0.8.2 wheel\n  (lattica_common/app_api.py sets Authorization: Bearer <token>).\ndescription: >-\n  Lattica does not publish an OpenAPI definition, so this profile was read off\n  the platform documentation and the official Python SDK rather than derived\n  from securitySchemes. There is no OAuth 2.0 and no OpenID Connect: the whole\n  platform authenticates with bearer tokens, but with TWO distinct token classes\n  that are easy to conflate — an organization-level management license and a\n  per-user, per-workload query token.\nbase_url: https://api.lattica.ai\noauth2: false\noidc: false\nmutual_tls:\
  \ false\n\nschemes:\n  - id: management_license\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <token>'\n    audience: Organization administrator\n    issued_by: Lattica web console (https://console.lattica.ai/)\n    grants: >-\n      Full management surface — create/activate/deactivate workloads (models),\n      generate and assign user access tokens, start/stop compute workers, read\n      account info, credits, and transaction history.\n    sdk_usage: 'LatticaManagement(\"your_license_from_lattica_console\")'\n    docs: https://platformdocs.lattica.ai/how-to-guides/access-control/how-to-create-user-access-token.md\n    expiration: Not documented.\n    rotation: Not documented.\n\n  - id: user_access_token\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: 'Authorization: Bearer <token>'\n    token_format: JWT\n    audience: End user querying a workload\n    issued_by: >-\n  \
  \    The workload service provider, via the web console (Token Management) or\n      the Python management SDK (generate_query_token).\n    scoping: >-\n      Bound to ONE user and ONE workload. A token may be created unassigned and\n      linked to a workload later; an end user cannot use an unassigned token.\n    grants: >-\n      Submit encrypted queries to the assigned workload, upload an evaluation\n      key, and retrieve the encrypted result. No management capability.\n    expiration: 30 days — tokens must be renewed on expiry.\n    retrievability: >-\n      Shown once at creation and NOT stored by the platform. It cannot be\n      retrieved later; a lost token must be replaced.\n    revocation: >-\n      Tokens can be updated, reassigned, deleted, or set active/cancelled from\n      the console or the management SDK\n      (update_token_info, assign_token_to_model, unassign_token_from_model,\n      delete_token).\n    docs: https://platformdocs.lattica.ai/architecture-overview/query-client.md\n\
  \nclient_side_cryptography:\n  note: >-\n    Distinct from authentication, but load-bearing for the trust model: the\n    bearer token authorizes the call, it does not grant access to plaintext.\n  secret_key: >-\n    Generated and held by the end user in the Query Client. Never sent to\n    Lattica. Encrypts the query input and decrypts the returned output.\n  evaluation_key: >-\n    Public key uploaded to the platform to accelerate homomorphic computation.\n    Does not permit decryption.\n  implication: >-\n    A compromised user access token allows an attacker to spend the token\n    holder's query budget against a workload, but not to read prior plaintext,\n    which never leaves the client.\n\nnot_supported:\n  - oauth2_authorization_code\n  - oauth2_client_credentials\n  - openid_connect\n  - api_key_query_parameter\n  - mutual_tls\n  - basic_auth\nscopes:\n  model: >-\n    No OAuth scope system. Authorization is coarse and structural — the token\n    class determines the capability\
  \ set, and the token-to-workload assignment\n    determines the resource. No scopes/ artifact is produced for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lattica/refs/heads/main/authentication/lattica-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Privacy
- Fully Homomorphic Encryption
- Encryption
- Confidential Computing
- Artificial Intelligence
- Machine Learning
- Inference
- Vector Search
- Security
---
