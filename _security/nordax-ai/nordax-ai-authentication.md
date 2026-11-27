---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nordax-ai-categories-api-openapi.yml
  format: yaml
  label: Nordax AI Categories API
  slug: nordax-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-categories-api-openapi.yml
- filename: nordax-ai-entities-api-openapi.yml
  format: yaml
  label: Nordax AI Entities API
  slug: nordax-ai-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-entities-api-openapi.yml
- filename: nordax-ai-netp-api-openapi.yml
  format: yaml
  label: Nordax AI Netp API
  slug: nordax-ai-netp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-netp-api-openapi.yml
- filename: nordax-ai-stats-api-openapi.yml
  format: yaml
  label: Nordax AI Stats API
  slug: nordax-ai-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nordax-ai/openapi/nordax-ai-stats-api-openapi.yml
auth_types: []
description: Authentication for Nordax AI API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nordax AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nordax AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nordax AI
provider_slug: nordax-ai
scheme_count: 1
schemes:
- evidence: All authenticated API requests use Bearer tokens.
  header: Authorization
  how_to_obtain: Generate an API key in the Dashboard → Settings → API Keys; the key has the prefix nak_ followed by 48 hex characters and is used as the bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: nordax-ai-authentication
source_filename: nordax-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.nordax.ai/developers/authentication
source_yaml: "generated: '2026-11-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.nordax.ai/developers/authentication\nsources:\n- https://www.nordax.ai/developers/authentication\n- https://www.nordax.ai/developers/api\n- https://www.nordax.ai/developers/platforms\ndescription: Authentication for Nordax AI API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All authenticated API requests use Bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the Dashboard → Settings → API Keys; the key has the prefix nak_ followed by 48 hex characters and is\n    used as the bearer token.\ndocs: https://www.nordax.ai/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/nordax-ai/authentication/nordax-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Identity
- Trust
- Platform
---
