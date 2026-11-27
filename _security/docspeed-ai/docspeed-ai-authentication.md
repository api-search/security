---
anonymous_access: false
api_key_in: []
api_specs:
- filename: docspeed-ai-agents-api-openapi.yml
  format: yaml
  label: Docspeed Agents API
  slug: docspeed-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-agents-api-openapi.yml
- filename: docspeed-ai-chat-api-openapi.yml
  format: yaml
  label: Docspeed Chat API
  slug: docspeed-ai-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-chat-api-openapi.yml
- filename: docspeed-ai-extraction-api-openapi.yml
  format: yaml
  label: Docspeed Extraction API
  slug: docspeed-ai-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-extraction-api-openapi.yml
- filename: docspeed-ai-files-api-openapi.yml
  format: yaml
  label: Docspeed Files API
  slug: docspeed-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-files-api-openapi.yml
- filename: docspeed-ai-generation-api-openapi.yml
  format: yaml
  label: Docspeed Generation API
  slug: docspeed-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-generation-api-openapi.yml
- filename: docspeed-ai-jobs-api-openapi.yml
  format: yaml
  label: Docspeed Jobs API
  slug: docspeed-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-jobs-api-openapi.yml
- filename: docspeed-ai-processing-api-openapi.yml
  format: yaml
  label: Docspeed Processing API
  slug: docspeed-ai-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/docspeed-ai/openapi/docspeed-ai-processing-api-openapi.yml
auth_types: []
description: Docspeed uses a simple bearer token for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Docspeed Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docspeed declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Docspeed
provider_slug: docspeed-ai
scheme_count: 1
schemes:
- evidence: 'Every public Docspeed customer API request uses bearer auth: Authorization: Bearer YOUR_DOCSPEED_API_KEY'
  header: Authorization
  how_to_obtain: Create or request an API key for the target workspace/environment and keep it server‑side.
  location: header
  name: Bearer token
  type: http-bearer
slug: docspeed-ai-authentication
source_filename: docspeed-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://api.docspeed.ai/docs/authentication-api-keys
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.docspeed.ai/docs/authentication-api-keys\nsources:\n- https://api.docspeed.ai/docs/authentication-api-keys\n- https://api.docspeed.ai/docs/quickstart\ndescription: Docspeed uses a simple bearer token for authentication.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every public Docspeed customer API request uses bearer auth: Authorization: Bearer YOUR_DOCSPEED_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or request an API key for the target workspace/environment and keep it server‑side.\ndocs: https://api.docspeed.ai/docs/authentication-api-keys\n"
source_yaml_url: https://artifacts.apis.io/docspeed-ai/authentication/docspeed-ai-authentication.yml
summary_line: 1 scheme
tags:
- AP Invoice Extraction
- BPO
- Shared Services
- Document AI
- Financial Services
- Procurement Automation
---
