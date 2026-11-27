---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aicontentdrop-com-account-api-openapi.yml
  format: yaml
  label: AI Content Drop Account API
  slug: aicontentdrop-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-account-api-openapi.yml
- filename: aicontentdrop-com-authentication-api-openapi.yml
  format: yaml
  label: AI Content Drop Authentication API
  slug: aicontentdrop-com-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-authentication-api-openapi.yml
- filename: aicontentdrop-com-batch-api-openapi.yml
  format: yaml
  label: AI Content Drop Batch API
  slug: aicontentdrop-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-batch-api-openapi.yml
- filename: aicontentdrop-com-discovery-api-openapi.yml
  format: yaml
  label: AI Content Drop Discovery API
  slug: aicontentdrop-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-discovery-api-openapi.yml
- filename: aicontentdrop-com-drops-api-openapi.yml
  format: yaml
  label: AI Content Drop Drops API
  slug: aicontentdrop-com-drops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-drops-api-openapi.yml
- filename: aicontentdrop-com-generation-api-openapi.yml
  format: yaml
  label: AI Content Drop Generation API
  slug: aicontentdrop-com-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-generation-api-openapi.yml
- filename: aicontentdrop-com-models-api-openapi.yml
  format: yaml
  label: AI Content Drop Models API
  slug: aicontentdrop-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicontentdrop-com/openapi/aicontentdrop-com-models-api-openapi.yml
auth_types: []
description: Authentication schemes as documented
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AI Content Drop Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Content Drop declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AI Content Drop
provider_slug: aicontentdrop-com
scheme_count: 1
schemes:
- evidence: 'Send Authorization: Bearer acd_live_… on any request that touches an account or spends credits.'
  header: Authorization
  how_to_obtain: Create a key in Settings → Integrations after signing in; keys are prefixed acd_live_.
  location: header
  name: API Key
  type: http-bearer
slug: aicontentdrop-com-authentication
source_filename: aicontentdrop-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aicontentdrop.com/docs/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aicontentdrop.com/docs/authentication\nsources:\n- https://aicontentdrop.com/docs/authentication\n- https://aicontentdrop.com/docs/authentication.md\n- https://aicontentdrop.com/auth.md\n- https://aicontentdrop.com/.well-known/http-message-signatures-directory\ndescription: Authentication schemes as documented\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send Authorization: Bearer acd_live_… on any request that touches an account or spends credits.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings → Integrations after signing in; keys are prefixed acd_live_.\ndocs: https://aicontentdrop.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/aicontentdrop-com/authentication/aicontentdrop-com-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Video
- Marketing
- Content Creation
- Software-as-a-Service
---
