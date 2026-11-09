---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bowmark-ai-library-api-openapi.yml
  format: yaml
  label: Bowmark AI Library API
  slug: bowmark-ai-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-library-api-openapi.yml
- filename: bowmark-ai-recipes-api-openapi.yml
  format: yaml
  label: Bowmark AI Recipes API
  slug: bowmark-ai-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-recipes-api-openapi.yml
- filename: bowmark-ai-run-api-openapi.yml
  format: yaml
  label: Bowmark AI Run API
  slug: bowmark-ai-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-run-api-openapi.yml
- filename: bowmark-ai-scripts-api-openapi.yml
  format: yaml
  label: Bowmark AI Scripts API
  slug: bowmark-ai-scripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-scripts-api-openapi.yml
- filename: bowmark-ai-sites-api-openapi.yml
  format: yaml
  label: Bowmark AI Sites API
  slug: bowmark-ai-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bowmark-ai/openapi/bowmark-ai-sites-api-openapi.yml
auth_types: []
description: Authentication for Bowmark AI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bowmark Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bowmark AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bowmark AI
provider_slug: bowmark-ai
scheme_count: 1
schemes:
- evidence: 'Every endpoint below takes the same header: Authorization: Bearer $BOWMARK_API_KEY'
  header: Authorization
  how_to_obtain: Sign up at bowmark.ai/sign-up, create a key at bowmark.ai/dashboard/keys, and use it as the Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: bowmark-ai-authentication
source_filename: bowmark-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://bowmark.ai/docs/installation
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bowmark.ai/docs/installation\nsources:\n- https://bowmark.ai/docs/installation\n- https://bowmark.ai/docs/http-api\n- https://bowmark.ai/docs/quickstart.md\n- https://bowmark.ai/docs/quickstart\ndescription: Authentication for Bowmark AI\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every endpoint below takes the same header: Authorization: Bearer $BOWMARK_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign up at bowmark.ai/sign-up, create a key at bowmark.ai/dashboard/keys, and use it as the Bearer token.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://bowmark.ai/docs/installation\n"
source_yaml_url: https://artifacts.apis.io/bowmark-ai/authentication/bowmark-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Automation
- Web
- Data Extraction
- Platform
- Company
---
