---
anonymous_access: false
api_key_in: []
api_specs:
- filename: modulos-ai-booking-api-openapi.yml
  format: yaml
  label: Modulos Booking API
  slug: modulos-ai-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-booking-api-openapi.yml
- filename: modulos-ai-evaluation-api-openapi.yml
  format: yaml
  label: Modulos Evaluation API
  slug: modulos-ai-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-evaluation-api-openapi.yml
- filename: modulos-ai-leads-api-openapi.yml
  format: yaml
  label: Modulos Leads API
  slug: modulos-ai-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modulos-ai/openapi/modulos-ai-leads-api-openapi.yml
auth_types: []
description: Authentication schemes as published on Modulos documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Modulos Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modulos declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Modulos
provider_slug: modulos-ai
scheme_count: 1
schemes:
- evidence: The Modulos Client uses an API token for authentication. Set the token as MODULOS_API_KEY in your environment.
  name: API token
  type: http-bearer
slug: modulos-ai-authentication
source_filename: modulos-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.modulos.ai/platform/integrations/api-tokens
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.modulos.ai/platform/integrations/api-tokens\nsources:\n- https://docs.modulos.ai/platform/integrations/api-tokens\n- https://docs.modulos.ai/guide/quickstart\n- https://docs.dev.modulos.ai/guide/quickstart\ndescription: Authentication schemes as published on Modulos documentation.\nschemes:\n- type: http-bearer\n  name: API token\n  evidence: The Modulos Client uses an API token for authentication. Set the token as MODULOS_API_KEY in your environment.\ndocs: https://docs.modulos.ai/platform/integrations/api-tokens\n"
source_yaml_url: https://artifacts.apis.io/modulos-ai/authentication/modulos-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI Governance
- Enterprise
- ISO 42001
- Risk Management
---
