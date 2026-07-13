---
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
- filename: celestia-p2p-api-openapi.yml
  format: yaml
  label: Celestia Node P2P API
  slug: celestia-p2p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/openapi/celestia-p2p-api-openapi.yml
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
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Celestia Authentication
name_suffix: Authentication
oauth_flows: []
overview: celestia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: celestia
provider_slug: celestia
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/celestia-blob-api-openapi.yml
  - openapi/celestia-blobstream-api-openapi.yml
  - openapi/celestia-da-api-openapi.yml
  - openapi/celestia-das-api-openapi.yml
  - openapi/celestia-fraud-api-openapi.yml
  - openapi/celestia-header-api-openapi.yml
  - openapi/celestia-node-api-openapi.yml
  - openapi/celestia-p2p-api-openapi.yml
  - openapi/celestia-share-api-openapi.yml
  - openapi/celestia-state-api-openapi.yml
  type: http
slug: celestia-authentication
source_filename: celestia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/celestia-blob-api-openapi.yml, openapi/celestia-blobstream-api-openapi.yml,\n  openapi/celestia-da-api-openapi.yml, openapi/celestia-das-api-openapi.yml, openapi/celestia-fraud-api-openapi.yml,\n  openapi/celestia-header-api-openapi.yml, openapi/celestia-node-api-openapi.yml, openapi/celestia-p2p-api-openapi.yml,\n  openapi/celestia-share-api-openapi.yml, openapi/celestia-state-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/celestia-blob-api-openapi.yml\n  - openapi/celestia-blobstream-api-openapi.yml\n  - openapi/celestia-da-api-openapi.yml\n  - openapi/celestia-das-api-openapi.yml\n  - openapi/celestia-fraud-api-openapi.yml\n  - openapi/celestia-header-api-openapi.yml\n  - openapi/celestia-node-api-openapi.yml\n  - openapi/celestia-p2p-api-openapi.yml\n  - openapi/celestia-share-api-openapi.yml\n  - openapi/celestia-state-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celestia/refs/heads/main/authentication/celestia-authentication.yml
summary_line: http · 1 scheme
tags: []
---
