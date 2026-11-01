---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hacktron-rest-api-cost-estimations-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Cost Estimations API
  slug: hacktron-rest-api-cost-estimations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-cost-estimations-api-openapi.yml
- filename: hacktron-rest-api-findings-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Findings API
  slug: hacktron-rest-api-findings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-findings-api-openapi.yml
- filename: hacktron-rest-api-hfw-api-openapi.yml
  format: yaml
  label: Hacktron REST API - HFW API
  slug: hacktron-rest-api-hfw-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-hfw-api-openapi.yml
- filename: hacktron-rest-api-repos-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Repos API
  slug: hacktron-rest-api-repos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-repos-api-openapi.yml
- filename: hacktron-rest-api-scans-api-openapi.yml
  format: yaml
  label: Hacktron REST API - Scans API
  slug: hacktron-rest-api-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hacktron/openapi/hacktron-rest-api-scans-api-openapi.yml
auth_types: []
description: Authentication schemes published for Hacktron
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hacktron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hacktron declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hacktron
provider_slug: hacktron
scheme_count: 1
schemes:
- evidence: The Hacktron REST API authenticates every request with an organization‑scoped API key sent in the `X-Api-Key` header.
  header: X-Api-Key
  how_to_obtain: API keys are created from the Hacktron dashboard (Settings → API keys) by an organization Admin or Owner.
  location: header
  name: API Key
  type: apiKey
slug: hacktron-authentication
source_filename: hacktron-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.hacktron.ai/api-reference/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.hacktron.ai/api-reference/authentication.md\nsources:\n- https://docs.hacktron.ai/api-reference/authentication.md\n- https://docs.hacktron.ai/code-review/setup.md\n- https://docs.hacktron.ai/white-box-pentest/quickstart.md\ndescription: Authentication schemes published for Hacktron\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Hacktron REST API authenticates every request with an organization‑scoped API key sent in the `X-Api-Key` header.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: API keys are created from the Hacktron dashboard (Settings → API keys) by an organization Admin or Owner.\nnote: No OAuth2, HTTP‑basic, bearer, JWT, HMAC, mTLS, or other schemes are documented on the provided pages.\ndocs: https://docs.hacktron.ai/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/hacktron/authentication/hacktron-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Automation
- Integration
- IoT
- Enterprise
---
