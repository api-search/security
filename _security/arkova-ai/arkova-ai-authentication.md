---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: arkova-ai-agents-api-openapi.yml
  format: yaml
  label: Arkova Agents API
  slug: arkova-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-agents-api-openapi.yml
- filename: arkova-ai-ai-intelligence-api-openapi.yml
  format: yaml
  label: Arkova AI Intelligence API
  slug: arkova-ai-ai-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-ai-intelligence-api-openapi.yml
- filename: arkova-ai-anchoring-api-openapi.yml
  format: yaml
  label: Arkova Anchoring API
  slug: arkova-ai-anchoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-anchoring-api-openapi.yml
- filename: arkova-ai-attestations-api-openapi.yml
  format: yaml
  label: Arkova Attestations API
  slug: arkova-ai-attestations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-attestations-api-openapi.yml
- filename: arkova-ai-compliance-api-openapi.yml
  format: yaml
  label: Arkova Compliance API
  slug: arkova-ai-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-compliance-api-openapi.yml
- filename: arkova-ai-folders-api-openapi.yml
  format: yaml
  label: Arkova Folders API
  slug: arkova-ai-folders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-folders-api-openapi.yml
- filename: arkova-ai-integrations-api-openapi.yml
  format: yaml
  label: Arkova Integrations API
  slug: arkova-ai-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-integrations-api-openapi.yml
- filename: arkova-ai-jobs-api-openapi.yml
  format: yaml
  label: Arkova Jobs API
  slug: arkova-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-jobs-api-openapi.yml
- filename: arkova-ai-key-management-api-openapi.yml
  format: yaml
  label: Arkova Key Management API
  slug: arkova-ai-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-key-management-api-openapi.yml
- filename: arkova-ai-organizations-api-openapi.yml
  format: yaml
  label: Arkova Organizations API
  slug: arkova-ai-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-organizations-api-openapi.yml
- filename: arkova-ai-search-api-openapi.yml
  format: yaml
  label: Arkova Search API
  slug: arkova-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-search-api-openapi.yml
- filename: arkova-ai-usage-api-openapi.yml
  format: yaml
  label: Arkova Usage API
  slug: arkova-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-usage-api-openapi.yml
- filename: arkova-ai-verification-api-openapi.yml
  format: yaml
  label: Arkova Verification API
  slug: arkova-ai-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-verification-api-openapi.yml
- filename: arkova-ai-webhooks-api-openapi.yml
  format: yaml
  label: Arkova Webhooks API
  slug: arkova-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arkova-ai/openapi/arkova-ai-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Arkova Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arkova secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arkova
provider_slug: arkova-ai
scheme_count: 2
schemes:
- description: 'API key as Bearer token: `Authorization: Bearer ak_live_...`'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/arkova-ai-openapi.json
  type: http
- description: 'API key via header: `X-API-Key: ak_live_...`'
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/arkova-ai-openapi.json
  type: apiKey
slug: arkova-ai-authentication
source_filename: arkova-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/arkova-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  description: 'API key as Bearer token: `Authorization: Bearer ak_live_...`'\n  sources:\n  - openapi/arkova-ai-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key via header: `X-API-Key: ak_live_...`'\n  sources:\n  - openapi/arkova-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/arkova-ai/authentication/arkova-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Trust
- Auditing
- Verification
- Records
- Agents
---
