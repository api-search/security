---
anonymous_access: false
api_key_in: []
api_specs:
- filename: giggal-ai-openapi-generated.yml
  format: yaml
  label: Giggal.ai API
  slug: giggal-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giggal-ai/openapi/_ae-authored/giggal-ai-openapi-generated.yml
auth_types: []
description: 'Authentication Pass your API key with every request via one of two headers. Either works. Option 1: Bearer token Authorization: Bearer tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx Option 2: X-API-Key header X-API-Key: tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Giggal.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Giggal.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Giggal.ai
provider_slug: giggal-ai
scheme_count: 2
schemes:
- evidence: 'Option 1: Bearer token Authorization: Bearer tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Option 2: X-API-Key header X-API-Key: tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'
  header: X-API-Key
  location: header
  name: X-API-Key
  type: apiKey
slug: giggal-ai-authentication
source_filename: giggal-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://giggal.ai/public/docs/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://giggal.ai/public/docs/authentication\nsources:\n- https://giggal.ai/public/docs/authentication\ndescription: 'Authentication Pass your API key with every request via one of two headers. Either works. Option 1: Bearer token Authorization:\n  Bearer tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx Option 2: X-API-Key header X-API-Key: tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Option 1: Bearer token Authorization: Bearer tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Option 2: X-API-Key header X-API-Key: tp_live_xxxxxxxxxxxxxxxxxxxxxxxxx'\n  location: header\n  header: X-API-Key\ndocs: https://giggal.ai/public/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/giggal-ai/authentication/giggal-ai-authentication.yml
summary_line: 2 schemes
tags:
- Email Verification
- Software-as-a-Service
- B2B
- Data Cleaning
- Technology
---
