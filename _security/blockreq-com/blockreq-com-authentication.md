---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blockreq-com-build-openapi-generated.yml
  format: yaml
  label: BlockReq build API
  slug: build-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockreq-com/openapi/_ae-authored/blockreq-com-build-openapi-generated.yml
- filename: blockreq-com-getting-started-openapi-generated.yml
  format: yaml
  label: BlockReq Getting Started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockreq-com/openapi/_ae-authored/blockreq-com-getting-started-openapi-generated.yml
auth_types: []
description: Authentication methods for BlockReq APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Blockreq Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlockReq declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: BlockReq
provider_slug: blockreq-com
scheme_count: 3
schemes:
- evidence: API keys are used to authenticate your requests to BlockReq's RPC endpoints.
  how_to_obtain: From the Dashboard → Endpoints → Add Endpoint; each endpoint shows its key and its HTTPS and WSS URLs.
  location: url
  name: RPC endpoint key
  type: apiKey
- evidence: 'Management API key (`akv1_…`): Dashboard → Settings → API Keys.'
  header: Authorization
  how_to_obtain: Dashboard → Settings → API Keys.
  location: header
  name: Management API key
  type: http-bearer
- authorize_url: https://blockreq.com/api/auth/authorize
  evidence: '`Authorization: Bearer <token>` on https://mcp.blockreq.com/mcp/account'
  header: Authorization
  how_to_obtain: User signs in to BlockReq, approves the client in a browser; uses Authorization Code flow with PKCE as described in the OAuth section.
  location: header
  name: OAuth access token
  scopes:
  - mcp:rpc.read
  - offline_access
  token_url: https://blockreq.com/api/auth/token
  type: http-bearer
slug: blockreq-com-authentication
source_filename: blockreq-com-authentication.yml
source_heading: Authentication Profile
source_url: https://blockreq.com/docs/getting-started/api-keys/
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://blockreq.com/docs/getting-started/api-keys/\nsources:\n- https://blockreq.com/docs/getting-started/api-keys/\n- https://blockreq.com/auth.md\n- https://blockreq.com/docs/getting-started/\n- https://blockreq.com/docs/getting-started/create-endpoint/\ndescription: Authentication methods for BlockReq APIs\nschemes:\n- type: apiKey\n  name: RPC endpoint key\n  evidence: API keys are used to authenticate your requests to BlockReq's RPC endpoints.\n  location: url\n  how_to_obtain: From the Dashboard → Endpoints → Add Endpoint; each endpoint shows its key and its HTTPS and WSS URLs.\n- type: http-bearer\n  name: Management API key\n  evidence: 'Management API key (`akv1_…`): Dashboard → Settings → API Keys.'\n  location: header\n  header: Authorization\n  how_to_obtain: Dashboard → Settings → API Keys.\n- type: http-bearer\n  name: OAuth access token\n  evidence: '`Authorization:\
  \ Bearer <token>` on https://mcp.blockreq.com/mcp/account'\n  location: header\n  header: Authorization\n  token_url: https://blockreq.com/api/auth/token\n  authorize_url: https://blockreq.com/api/auth/authorize\n  scopes:\n  - mcp:rpc.read\n  - offline_access\n  how_to_obtain: User signs in to BlockReq, approves the client in a browser; uses Authorization Code flow with PKCE as described in the OAuth\n    section.\ndocs: https://blockreq.com/docs/getting-started/api-keys/\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/blockreq-com/authentication/blockreq-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Blockchain
- RPC
- EVM
- Infrastructure
- Developer Tools
---
