---
api_key_in: []
api_specs:
- filename: ipfs-kubo-rpc-api.json
  format: json
  label: IPFS Kubo RPC API
  slug: ipfs-kubo-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/openapi/ipfs-kubo-rpc-api.json
- filename: ipfs-pinning-service-api.yaml
  format: yaml
  label: IPFS Pinning Service API
  slug: ipfs-pinning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/openapi/ipfs-pinning-service-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ipfs Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPFS secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IPFS
provider_slug: ipfs
scheme_count: 1
schemes:
- description: 'An opaque token is required to be sent with each request in the HTTP header:

    - `Authorization: Bearer <access-token>`


    The `access-token` should be generated per device, and the user should have the ability to revoke each token separately.'
  name: accessToken
  scheme: bearer
  sources:
  - openapi/ipfs-pinning-service-api.yaml
  type: http
slug: ipfs-authentication
source_filename: ipfs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ipfs-pinning-service-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessToken\n  type: http\n  scheme: bearer\n  description: |-\n    An opaque token is required to be sent with each request in the HTTP header:\n    - `Authorization: Bearer <access-token>`\n\n    The `access-token` should be generated per device, and the user should have the ability to revoke each token separately.\n  sources:\n  - openapi/ipfs-pinning-service-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/authentication/ipfs-authentication.yml
summary_line: http · 1 scheme
tags:
- IPFS
- Distributed Storage
- Content-Addressed
- Decentralized
- Peer-to-Peer
- File Storage
- DAG
- Pinning
- Gateway
---
