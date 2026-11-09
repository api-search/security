---
anonymous_access: false
api_key_in: []
api_specs:
- filename: deepsfetch-com-api-openapi.json
  format: json
  label: DeepSFetch API API
  slug: deepsfetch-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deepsfetch-com/openapi/_original/deepsfetch-com-api-openapi.json
auth_types: []
description: Authentication schemes for DeepSFetch API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Deepsfetch Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DeepSFetch declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DeepSFetch
provider_slug: deepsfetch-com
scheme_count: 1
schemes:
- evidence: Machine calls use Bearer; a dashboard session does not replace an external key.
  header: Authorization
  how_to_obtain: Create an API key in the API Keys section of the workspace and use it as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: deepsfetch-com-authentication
source_filename: deepsfetch-com-authentication.yml
source_heading: Authentication Profile
source_url: https://deepsfetch.com/docs/authentication?lang=pt-BR
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://deepsfetch.com/docs/authentication?lang=pt-BR\nsources:\n- https://deepsfetch.com/docs/authentication?lang=pt-BR\n- https://deepsfetch.com/docs/authentication\n- https://deepsfetch.com/docs/webhooks\n- https://deepsfetch.com/docs/getting-started?lang=pt-BR\ndescription: Authentication schemes for DeepSFetch API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Machine calls use Bearer; a dashboard session does not replace an external key.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the API Keys section of the workspace and use it as the Bearer token.\ndocs: https://deepsfetch.com/docs/authentication?lang=pt-BR\n"
source_yaml_url: https://artifacts.apis.io/deepsfetch-com/authentication/deepsfetch-com-authentication.yml
summary_line: 1 scheme
tags:
- Data Extraction
- AI Integration
- Monitoring
- Collection
---
