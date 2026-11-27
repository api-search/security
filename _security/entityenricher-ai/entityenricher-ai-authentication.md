---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entityenricher-ai-openapi-generated.yml
  format: yaml
  label: Entity Enricher API
  slug: entityenricher-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entityenricher-ai/openapi/_ae-authored/entityenricher-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Entity Enricher
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Entity Enricher Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entity Enricher declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Entity Enricher
provider_slug: entityenricher-ai
scheme_count: 2
schemes:
- evidence: 'Send your API key in the X-API-Key header with every request: curl -H "X-API-Key: ent_your_key_here"'
  header: X-API-Key
  how_to_obtain: Create organization access keys via the API Keys page or programmatically via POST /api/auth/api-keys.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'The API supports two authentication methods: Bearer JWT tokens for web clients, and API keys (format: ent_XXXX ) for programmatic access via the X-API-Key header.'
  header: Authorization
  how_to_obtain: Obtain a JWT token through the web client login flow (details not provided on the pages).
  location: header
  name: Bearer JWT
  type: http-bearer
slug: entityenricher-ai-authentication
source_filename: entityenricher-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://entityenricher.ai/docs/platform/api-keys
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://entityenricher.ai/docs/platform/api-keys\nsources:\n- https://entityenricher.ai/docs/platform/api-keys\n- https://entityenricher.ai/docs/api\n- https://entityenricher.ai/docs\ndescription: Authentication methods for Entity Enricher\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'Send your API key in the X-API-Key header with every request: curl -H \"X-API-Key: ent_your_key_here\"'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create organization access keys via the API Keys page or programmatically via POST /api/auth/api-keys.\n- type: http-bearer\n  name: Bearer JWT\n  evidence: 'The API supports two authentication methods: Bearer JWT tokens for web clients, and API keys (format: ent_XXXX ) for programmatic\n    access via the X-API-Key header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a JWT token through the web client\
  \ login flow (details not provided on the pages).\nnote: No OAuth2 flows are described on the provided pages.\ndocs: https://entityenricher.ai/docs/platform/api-keys\n"
source_yaml_url: https://artifacts.apis.io/entityenricher-ai/authentication/entityenricher-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Data Enrichment
- Platform
- Automation
- Database
---
