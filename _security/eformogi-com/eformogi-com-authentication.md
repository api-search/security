---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: eformogi-com-account-api-openapi.yml
  format: yaml
  label: Eformogi Account API
  slug: eformogi-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-account-api-openapi.yml
- filename: eformogi-com-admin-api-openapi.yml
  format: yaml
  label: Eformogi Admin API
  slug: eformogi-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-admin-api-openapi.yml
- filename: eformogi-com-agent-protocol-api-openapi.yml
  format: yaml
  label: Eformogi Agent Protocol API
  slug: eformogi-com-agent-protocol-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-agent-protocol-api-openapi.yml
- filename: eformogi-com-consent-api-openapi.yml
  format: yaml
  label: Eformogi Consent API
  slug: eformogi-com-consent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-consent-api-openapi.yml
- filename: eformogi-com-documents-api-openapi.yml
  format: yaml
  label: Eformogi Documents API
  slug: eformogi-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-documents-api-openapi.yml
- filename: eformogi-com-family-api-openapi.yml
  format: yaml
  label: Eformogi Family API
  slug: eformogi-com-family-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-family-api-openapi.yml
- filename: eformogi-com-issuer-api-openapi.yml
  format: yaml
  label: Eformogi Issuer API
  slug: eformogi-com-issuer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-issuer-api-openapi.yml
- filename: eformogi-com-public-api-openapi.yml
  format: yaml
  label: Eformogi Public API
  slug: eformogi-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-public-api-openapi.yml
- filename: eformogi-com-schema-api-openapi.yml
  format: yaml
  label: Eformogi Schema API
  slug: eformogi-com-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-schema-api-openapi.yml
- filename: eformogi-com-sharing-api-openapi.yml
  format: yaml
  label: Eformogi Sharing API
  slug: eformogi-com-sharing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-sharing-api-openapi.yml
- filename: eformogi-com-system-api-openapi.yml
  format: yaml
  label: Eformogi System API
  slug: eformogi-com-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-system-api-openapi.yml
- filename: eformogi-com-trust-api-openapi.yml
  format: yaml
  label: Eformogi Trust API
  slug: eformogi-com-trust-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eformogi-com/openapi/eformogi-com-trust-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Eformogi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eformogi secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Eformogi
provider_slug: eformogi-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Supabase JWT access token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/eformogi-com-openapi.json
  type: http
- description: Institutional org API key. Use "Bearer efg_org_..." or "Api-Key efg_org_..." header. Keys are scoped to specific data categories.
  in: header
  name: orgApiKey
  parameter: Authorization
  sources:
  - openapi/eformogi-com-openapi.json
  type: apiKey
slug: eformogi-com-authentication
source_filename: eformogi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: derived\nsource: openapi/eformogi-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Supabase JWT access token\n  sources:\n  - openapi/eformogi-com-openapi.json\n- name: orgApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Institutional org API key. Use \"Bearer efg_org_...\" or \"Api-Key efg_org_...\"\n    header. Keys are scoped to specific data categories.\n  sources:\n  - openapi/eformogi-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/eformogi-com/authentication/eformogi-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Transcript
- Free
- Privacy
- Open Standard
---
