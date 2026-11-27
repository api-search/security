---
anonymous_access: false
api_key_in: []
api_specs:
- filename: heyresearch-xyz-agents-api-openapi.yml
  format: yaml
  label: HEY Research Lab Agents API
  slug: heyresearch-xyz-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-agents-api-openapi.yml
- filename: heyresearch-xyz-contracts-api-openapi.yml
  format: yaml
  label: HEY Research Lab Contracts API
  slug: heyresearch-xyz-contracts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-contracts-api-openapi.yml
- filename: heyresearch-xyz-evidence-api-openapi.yml
  format: yaml
  label: HEY Research Lab Evidence API
  slug: heyresearch-xyz-evidence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-evidence-api-openapi.yml
- filename: heyresearch-xyz-hey-api-openapi.yml
  format: yaml
  label: HEY Research Lab Hey API
  slug: heyresearch-xyz-hey-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-hey-api-openapi.yml
- filename: heyresearch-xyz-market-api-openapi.yml
  format: yaml
  label: HEY Research Lab Market API
  slug: heyresearch-xyz-market-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-market-api-openapi.yml
- filename: heyresearch-xyz-partners-api-openapi.yml
  format: yaml
  label: HEY Research Lab Partners API
  slug: heyresearch-xyz-partners-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-partners-api-openapi.yml
- filename: heyresearch-xyz-projects-api-openapi.yml
  format: yaml
  label: HEY Research Lab Projects API
  slug: heyresearch-xyz-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-projects-api-openapi.yml
- filename: heyresearch-xyz-research-api-openapi.yml
  format: yaml
  label: HEY Research Lab Research API
  slug: heyresearch-xyz-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-research-api-openapi.yml
- filename: heyresearch-xyz-status-api-openapi.yml
  format: yaml
  label: HEY Research Lab Status API
  slug: heyresearch-xyz-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heyresearch-xyz/openapi/heyresearch-xyz-status-api-openapi.yml
auth_types: []
description: Authentication for HEY Research Lab API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HEY Research Lab Authentication
name_suffix: Authentication
oauth_flows: []
overview: HEY Research Lab declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HEY Research Lab
provider_slug: heyresearch-xyz
scheme_count: 1
schemes:
- evidence: 'A key is optional. A free key from your account page takes a minute and needs no holding: it names your product to HEY, carries a monthly allowance and unlocks the bulk reads below. Send it as authorization: Bearer hey_… .'
  header: Authorization
  how_to_obtain: Create a free API key on the account page; the key is returned as a bearer token prefixed with "hey_".
  location: header
  name: HEY API Key
  type: http-bearer
slug: heyresearch-xyz-authentication
source_filename: heyresearch-xyz-authentication.yml
source_heading: Authentication Profile
source_url: https://heyresearch.xyz/docs/research-economy
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://heyresearch.xyz/docs/research-economy\nsources:\n- https://heyresearch.xyz/docs/research-economy\n- https://heyresearch.xyz/docs/integrations\n- https://heyresearch.xyz/docs/hey-token\n- https://heyresearch.xyz/developers\ndescription: Authentication for HEY Research Lab API\nschemes:\n- type: http-bearer\n  name: HEY API Key\n  evidence: 'A key is optional. A free key from your account page takes a minute and needs no holding: it names your product to HEY, carries a\n    monthly allowance and unlocks the bulk reads below. Send it as authorization: Bearer hey_… .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a free API key on the account page; the key is returned as a bearer token prefixed with \"hey_\".\ndocs: https://heyresearch.xyz/docs/research-economy\n"
source_yaml_url: https://artifacts.apis.io/heyresearch-xyz/authentication/heyresearch-xyz-authentication.yml
summary_line: 1 scheme
tags:
- Blockchain
- Data
- Decentralized Finance
- Community
---
