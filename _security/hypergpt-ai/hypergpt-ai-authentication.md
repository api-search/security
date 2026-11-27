---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as documented on HyperGPT pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: HyperGPT Authentication
name_suffix: Authentication
oauth_flows: []
overview: HyperGPT declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: HyperGPT
provider_slug: hypergpt-ai
scheme_count: 2
schemes:
- evidence: Your newly generated API key is ready to use. Use this key to authenticate your requests.
  how_to_obtain: Navigate to the HyperStore page, go to Developer Resources and API Access, and click the 'GENERATE API KEY' button.
  name: API Key
  type: apiKey
- evidence: The Get Token endpoint facilitates the processing of a given token, subsequently returning a new token for the user.
  how_to_obtain: Provide an existing JWT in the 'token' query parameter to the Get Token endpoint.
  location: query
  name: User Token
  token_url: https://sdk.hypergpt.ai/user/get_token
  type: http-bearer
slug: hypergpt-ai-authentication
source_filename: hypergpt-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hypergpt.ai/docs/products/1-1-how-to-get-api-key
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hypergpt.ai/docs/products/1-1-how-to-get-api-key\nsources:\n- https://www.hypergpt.ai/docs/products/1-1-how-to-get-api-key\n- https://www.hypergpt.ai/docs/products/1-2-get-token\n- https://www.hypergpt.ai/docs/ecosystem/hgpt-token\ndescription: Authentication methods as documented on HyperGPT pages.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Your newly generated API key is ready to use. Use this key to authenticate your requests.\n  how_to_obtain: Navigate to the HyperStore page, go to Developer Resources and API Access, and click the 'GENERATE API KEY' button.\n- type: http-bearer\n  name: User Token\n  evidence: The Get Token endpoint facilitates the processing of a given token, subsequently returning a new token for the user.\n  location: query\n  token_url: https://sdk.hypergpt.ai/user/get_token\n  how_to_obtain: Provide an existing JWT in the 'token'\
  \ query parameter to the Get Token endpoint.\ndocs: https://www.hypergpt.ai/docs/products/1-1-how-to-get-api-key\n"
source_yaml_url: https://artifacts.apis.io/hypergpt-ai/authentication/hypergpt-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Web3
- Ecosystem
- Platform
- Tools
---
