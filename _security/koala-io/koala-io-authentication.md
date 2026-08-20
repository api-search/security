---
api_key_in: []
api_specs:
- filename: koala-io-accounts-api-openapi.yml
  format: yaml
  label: Koala Accounts API
  slug: koala-io-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-accounts-api-openapi.yml
- filename: koala-io-collection-api-openapi.yml
  format: yaml
  label: Koala Collection API
  slug: koala-io-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-collection-api-openapi.yml
- filename: koala-io-deletion-api-openapi.yml
  format: yaml
  label: Koala Deletion API
  slug: koala-io-deletion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-deletion-api-openapi.yml
- filename: koala-io-sdk-api-openapi.yml
  format: yaml
  label: Koala SDK API
  slug: koala-io-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/openapi/koala-io-sdk-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Koala Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koala secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koala
provider_slug: koala-io
scheme_count: 1
schemes:
- bearerFormat: sk_
  description: 'Secret API key created in Settings -> API Keys, sent as `Authorization: Bearer sk_...`. Used only by the Deletion (GDPR) API.'
  name: SecretApiKey
  scheme: bearer
  sources:
  - openapi/koala-io-accounts-api-openapi.yml
  - openapi/koala-io-collection-api-openapi.yml
  - openapi/koala-io-deletion-api-openapi.yml
  - openapi/koala-io-sdk-api-openapi.yml
  type: http
slug: koala-io-authentication
source_filename: koala-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: openapi/koala-io-accounts-api-openapi.yml, openapi/koala-io-collection-api-openapi.yml,\n  openapi/koala-io-deletion-api-openapi.yml, openapi/koala-io-sdk-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: SecretApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: sk_\n  description: 'Secret API key created in Settings -> API Keys, sent as `Authorization: Bearer\n    sk_...`. Used only by the Deletion (GDPR) API.'\n  sources:\n  - openapi/koala-io-accounts-api-openapi.yml\n  - openapi/koala-io-collection-api-openapi.yml\n  - openapi/koala-io-deletion-api-openapi.yml\n  - openapi/koala-io-sdk-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koala-io/refs/heads/main/authentication/koala-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Buyer Intent
- Visitor Identification
- De-anonymization
- Enrichment
- Go-To-Market
- Sales Intelligence
- B2B
---
