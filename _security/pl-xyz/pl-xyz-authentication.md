---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pl-xyz-openapi-generated.yml
  format: yaml
  label: Protocol Labs API
  slug: pl-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pl-xyz/openapi/_ae-authored/pl-xyz-openapi-generated.yml
auth_types: []
description: Secure Kubo RPC with TLS and HTTP Auth
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pl Xyz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Protocol Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Protocol Labs
provider_slug: pl-xyz
scheme_count: 1
schemes:
- evidence: 'Authentication: Basic HTTP authentication for the Kubo RPC API .'
  how_to_obtain: 'Set the AuthSecret in the Kubo config, e.g., "AuthSecret": "basic:hello:world123", and use the credentials with the --api-auth flag or embed them in the URL (https://hello:world123@YOUR_DOMAIN).'
  name: basic
  type: http-basic
slug: pl-xyz-authentication
source_filename: pl-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ipfs.tech/how-to/kubo-rpc-tls-auth/
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ipfs.tech/how-to/kubo-rpc-tls-auth/\nsources:\n- https://docs.ipfs.tech/how-to/kubo-rpc-tls-auth/\n- https://docs.ipfs.tech/how-to/command-line-quick-start/\n- https://docs.ipfs.tech/quickstart/pin-cli/\n- https://docs.ipfs.tech/quickstart/retrieve/\ndescription: Secure Kubo RPC with TLS and HTTP Auth\nschemes:\n- type: http-basic\n  name: basic\n  evidence: 'Authentication: Basic HTTP authentication for the Kubo RPC API .'\n  how_to_obtain: 'Set the AuthSecret in the Kubo config, e.g., \"AuthSecret\": \"basic:hello:world123\", and use the credentials with the --api-auth\n    flag or embed them in the URL (https://hello:world123@YOUR_DOMAIN).'\nnote: No OAuth2, bearer, API key, or other authentication schemes are documented on the referenced pages.\ndocs: https://docs.ipfs.tech/how-to/kubo-rpc-tls-auth/\n"
source_yaml_url: https://artifacts.apis.io/pl-xyz/authentication/pl-xyz-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Decentralized
- OpenSource
- Web3
- Infrastructure
---
