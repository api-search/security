---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bynn-com-age-verification-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Age Verification API
  slug: bynn-com-age-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-age-verification-api-openapi.yml
- filename: bynn-com-aml-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Aml API
  slug: bynn-com-aml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-aml-api-openapi.yml
- filename: bynn-com-api-keys-api-openapi.yml
  format: yaml
  label: Bynn Intelligence API Keys API
  slug: bynn-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-api-keys-api-openapi.yml
- filename: bynn-com-autodoc-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Autodoc API
  slug: bynn-com-autodoc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-autodoc-api-openapi.yml
- filename: bynn-com-documents-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Documents API
  slug: bynn-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-documents-api-openapi.yml
- filename: bynn-com-dossiers-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Dossiers API
  slug: bynn-com-dossiers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-dossiers-api-openapi.yml
- filename: bynn-com-face-collections-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Collections API
  slug: bynn-com-face-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-collections-api-openapi.yml
- filename: bynn-com-face-enrollment-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Enrollment API
  slug: bynn-com-face-enrollment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-enrollment-api-openapi.yml
- filename: bynn-com-face-search-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Face Search API
  slug: bynn-com-face-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-face-search-api-openapi.yml
- filename: bynn-com-moderation-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Moderation API
  slug: bynn-com-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-moderation-api-openapi.yml
- filename: bynn-com-nfc-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Nfc API
  slug: bynn-com-nfc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-nfc-api-openapi.yml
- filename: bynn-com-sessions-api-openapi.yml
  format: yaml
  label: Bynn Intelligence Sessions API
  slug: bynn-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bynn-com/openapi/bynn-com-sessions-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Bynn Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bynn Intelligence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bynn Intelligence
provider_slug: bynn-com
scheme_count: 1
schemes:
- description: Enter your PRIVATE KEY token prefixed with `Bearer `, e.g. `Bearer your_token_here`
  in: header
  name: PrivateKey
  parameter: Authorization
  sources:
  - openapi/bynn-com-openapi.json
  type: apiKey
slug: bynn-com-authentication
source_filename: bynn-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/bynn-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PrivateKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Enter your PRIVATE KEY token prefixed with `Bearer `, e.g. `Bearer your_token_here`\n  sources:\n  - openapi/bynn-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/bynn-com/authentication/bynn-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Enterprise
- Frontier Research
- Identity Verification
- Digital Trust
---
