---
api_key_in:
- header
api_specs:
- filename: story-protocol-collections-api-openapi.yml
  format: yaml
  label: Story Protocol Collections API
  slug: story-protocol-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-collections-api-openapi.yml
- filename: story-protocol-disputes-api-openapi.yml
  format: yaml
  label: Story Protocol Disputes API
  slug: story-protocol-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-disputes-api-openapi.yml
- filename: story-protocol-ipassets-api-openapi.yml
  format: yaml
  label: Story Protocol IPAssets API
  slug: story-protocol-ipassets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-ipassets-api-openapi.yml
- filename: story-protocol-ipgroup-api-openapi.yml
  format: yaml
  label: Story Protocol IPGroup API
  slug: story-protocol-ipgroup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-ipgroup-api-openapi.yml
- filename: story-protocol-iplicenseterms-api-openapi.yml
  format: yaml
  label: Story Protocol IPLicenseTerms API
  slug: story-protocol-iplicenseterms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-iplicenseterms-api-openapi.yml
- filename: story-protocol-licenses-api-openapi.yml
  format: yaml
  label: Story Protocol Licenses API
  slug: story-protocol-licenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licenses-api-openapi.yml
- filename: story-protocol-licensetemplates-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTemplates API
  slug: story-protocol-licensetemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licensetemplates-api-openapi.yml
- filename: story-protocol-licenseterms-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTerms API
  slug: story-protocol-licenseterms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licenseterms-api-openapi.yml
- filename: story-protocol-licensetokens-api-openapi.yml
  format: yaml
  label: Story Protocol LicenseTokens API
  slug: story-protocol-licensetokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-licensetokens-api-openapi.yml
- filename: story-protocol-modules-api-openapi.yml
  format: yaml
  label: Story Protocol Modules API
  slug: story-protocol-modules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-modules-api-openapi.yml
- filename: story-protocol-permissions-api-openapi.yml
  format: yaml
  label: Story Protocol Permissions API
  slug: story-protocol-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-permissions-api-openapi.yml
- filename: story-protocol-royalties-api-openapi.yml
  format: yaml
  label: Story Protocol Royalties API
  slug: story-protocol-royalties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-royalties-api-openapi.yml
- filename: story-protocol-transactions-api-openapi.yml
  format: yaml
  label: Story Protocol Transactions API
  slug: story-protocol-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/openapi/story-protocol-transactions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Story Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Story Protocol secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Story Protocol
provider_slug: story-protocol
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/story-protocol-openapi-original.json
  type: apiKey
slug: story-protocol-authentication
source_filename: story-protocol-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/story-protocol-openapi-original.json\ndocs: https://docs.story.foundation/api-reference/protocol/introduction\nnotes: >-\n  Authentication is a static API key in the X-Api-Key header. Every request also\n  requires an X-Chain header selecting the network (mainnet = Story chain 1514,\n  aeneid = testnet chain 1315). Story publishes shared public keys (see\n  sandbox/story-protocol-sandbox.yml); higher rate limits are granted via the\n  Builder Discord. No OAuth/OIDC.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/story-protocol-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/story-protocol/refs/heads/main/authentication/story-protocol-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Blockchain
- Intellectual Property
- Licensing
- Royalties
- Web3
- NFT
- Developer Tools
---
