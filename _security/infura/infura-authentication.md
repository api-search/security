---
api_key_in:
- query
api_specs:
- filename: infura-asyncapi.yml
  format: yaml
  label: Infura JSON-RPC API
  slug: json-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/infura/refs/heads/main/asyncapi/infura-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Infura Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infura secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Infura
provider_slug: infura
scheme_count: 1
schemes:
- description: 'Infura API keys are passed as a path segment in the server URL

    (https://mainnet.infura.io/v3/<YOUR-API-KEY>), not as a query parameter

    or header. This security scheme is a documentation hint only.'
  in: query
  name: ApiKeyInPath
  parameter: apiKey
  sources:
  - openapi/infura-openapi.yml
  type: apiKey
slug: infura-authentication
source_filename: infura-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/infura-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyInPath\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: |-\n    Infura API keys are passed as a path segment in the server URL\n    (https://mainnet.infura.io/v3/<YOUR-API-KEY>), not as a query parameter\n    or header. This security scheme is a documentation hint only.\n  sources:\n  - openapi/infura-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infura/refs/heads/main/authentication/infura-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Web3
- Blockchain
- RPC
- Infrastructure
- MetaMask
- ConsenSys
---
