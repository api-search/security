---
anonymous_access: false
api_key_in: []
api_specs:
- filename: celestia-blob-api-openapi.yml
  format: yaml
  label: Celestia Node Blob API
  slug: celestia-blob-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-blob-api-openapi.yml
- filename: celestia-header-api-openapi.yml
  format: yaml
  label: Celestia Node Header API
  slug: celestia-header-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-header-api-openapi.yml
- filename: celestia-da-api-openapi.yml
  format: yaml
  label: Celestia Node DA API
  slug: celestia-da-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-da-api-openapi.yml
- filename: celestia-share-api-openapi.yml
  format: yaml
  label: Celestia Node Share API
  slug: celestia-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-share-api-openapi.yml
- filename: celestia-state-api-openapi.yml
  format: yaml
  label: Celestia Node State API
  slug: celestia-state-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-state-api-openapi.yml
- filename: celestia-das-api-openapi.yml
  format: yaml
  label: Celestia Node DAS API
  slug: celestia-das-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-das-api-openapi.yml
- filename: celestia-fraud-api-openapi.yml
  format: yaml
  label: Celestia Node Fraud API
  slug: celestia-fraud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-fraud-api-openapi.yml
- filename: celestia-node-api-openapi.yml
  format: yaml
  label: Celestia Node Admin API
  slug: celestia-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-node-api-openapi.yml
- filename: celestia-blobstream-api-openapi.yml
  format: yaml
  label: Celestia Node Blobstream API
  slug: celestia-blobstream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-blobstream-api-openapi.yml
- filename: celestia-p2-p-api-openapi.yml
  format: yaml
  label: Celestia P2 P API
  slug: celestia-p2-p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-p2-p-api-openapi.yml
auth_types:
- http
description: The Celestia Node API authenticates with a single HTTP bearer token, but the interesting part is not the scheme — it is who issues it and what it carries. The token is a JWT minted by the operator's own node through the `celestia <node_type> auth <level>` CLI (or node.AuthNew over an already-authorized connection), not by any Celestia Labs service. There is no vendor account, no API key to rotate in a dashboard, and no authorization server. Each token encodes one of four capability levels, and the provider declares the required level per method inside its OpenRPC document — which makes this a genuinely machine-readable permission model even though it is not OAuth.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Celestia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Celestia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Celestia
provider_slug: celestia
scheme_count: 1
schemes:
- format: JWT
  header: 'Authorization: Bearer <token>'
  issuer: the operator's own celestia-node instance
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/celestia-node-api-openrpc.json
  - openapi/celestia-blob-api-openapi.yml
  - openapi/celestia-blobstream-api-openapi.yml
  - openapi/celestia-da-api-openapi.yml
  - openapi/celestia-das-api-openapi.yml
  - openapi/celestia-fraud-api-openapi.yml
  - openapi/celestia-header-api-openapi.yml
  - openapi/celestia-node-api-openapi.yml
  - openapi/celestia-p2-p-api-openapi.yml
  - openapi/celestia-share-api-openapi.yml
  - openapi/celestia-state-api-openapi.yml
  type: http
slug: celestia-authentication
source_filename: celestia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\ndocs: https://docs.celestia.org/build/rpc/node-api.md\nsource: >-\n  https://docs.celestia.org/build/rpc/node-api.md,\n  https://docs.celestia.org/operate/data-availability/light-node/advanced.md,\n  openapi/celestia-node-api-openrpc.json,\n  openapi/celestia-blob-api-openapi.yml, openapi/celestia-blobstream-api-openapi.yml,\n  openapi/celestia-da-api-openapi.yml, openapi/celestia-das-api-openapi.yml,\n  openapi/celestia-fraud-api-openapi.yml, openapi/celestia-header-api-openapi.yml,\n  openapi/celestia-node-api-openapi.yml, openapi/celestia-p2-p-api-openapi.yml,\n  openapi/celestia-share-api-openapi.yml, openapi/celestia-state-api-openapi.yml\ndescription: >-\n  The Celestia Node API authenticates with a single HTTP bearer token, but the interesting\n  part is not the scheme — it is who issues it and what it carries. The token is a JWT minted\n  by the operator's own node through the `celestia <node_type> auth <level>` CLI (or\n \
  \ node.AuthNew over an already-authorized connection), not by any Celestia Labs service.\n  There is no vendor account, no API key to rotate in a dashboard, and no authorization\n  server. Each token encodes one of four capability levels, and the provider declares the\n  required level per method inside its OpenRPC document — which makes this a genuinely\n  machine-readable permission model even though it is not OAuth.\nsummary:\n  types:\n  - http\n  vendor_issued: false\n  self_issued: true\n  scopes_machine_readable: true\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  format: JWT\n  header: 'Authorization: Bearer <token>'\n  issuer: the operator's own celestia-node instance\n  sources:\n  - openapi/celestia-node-api-openrpc.json\n  - openapi/celestia-blob-api-openapi.yml\n  - openapi/celestia-blobstream-api-openapi.yml\n  - openapi/celestia-da-api-openapi.yml\n  - openapi/celestia-das-api-openapi.yml\n  - openapi/celestia-fraud-api-openapi.yml\n  - openapi/celestia-header-api-openapi.yml\n\
  \  - openapi/celestia-node-api-openapi.yml\n  - openapi/celestia-p2-p-api-openapi.yml\n  - openapi/celestia-share-api-openapi.yml\n  - openapi/celestia-state-api-openapi.yml\nissuance:\n  cli: celestia <node_type> auth <public|read|write|admin> --p2p.network <network>\n  example: celestia light auth admin --p2p.network mocha\n  rpc: node.AuthNew\n  verification_rpc: node.AuthVerify\n  skip_auth_flag: --rpc.skip-auth\n  note: >-\n    Each invocation mints a NEW token; the CLI does not return an existing one.\npermission_levels:\n- level: public\n  description: Methods callable without a token.\n- level: read\n  description: Read-only access across the data surface.\n  method_count: 41\n- level: write\n  description: Submitting blobs and state transactions.\n  method_count: 12\n- level: admin\n  description: Node administration, including the whole p2p module and key node.* methods.\n  method_count: 27\nlevel_declared_per_method: true\nlevel_evidence: >-\n  Every method in openrpc-v0.31.4.json\
  \ carries its requirement in the description field, as\n  \"Auth level: read. Requests must include the HTTP header: Authorization: Bearer <token>.\"\n  Counts above were computed across all 80 methods.\nlevel_by_module:\n  blob:\n    read: 6\n    write: 1\n  blobstream:\n    read: 2\n  da:\n    read: 6\n    write: 2\n  das:\n    read: 2\n  header:\n    read: 10\n  node:\n    admin: 5\n    read: 1\n  p2p:\n    admin: 22\n  share:\n    read: 7\n  state:\n    read: 7\n    write: 9\noauth2: false\nopenid_connect: false\nmtls: false\nrevocation:\n  supported: false\n  evidence: >-\n    \"Each time you run this, you will receive a new token. It's not possible to revoke\n    tokens once they are issued.\" — https://docs.celestia.org/operate/data-availability/light-node/advanced.md\n  consequence: >-\n    A leaked admin token grants permanent control of the node's libp2p and administrative\n    surface until the node's JWT signing key is rotated. For an agent deployment this is the\n    single\
  \ sharpest operational risk on the API: issue read-level tokens by default and mint\n    write or admin only for the specific job that needs them.\nexpiry:\n  published: false\n  note: No token lifetime or expiry policy is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/authentication/celestia-authentication.yml
summary_line: http · 1 scheme
tags:
- Blockchain
- Data Availability
- Web3
- Infrastructure
- Open-Source
- JSON-RPC
- Modular Blockchain
- Rollup
- Cryptography
- Developer Tools
---
