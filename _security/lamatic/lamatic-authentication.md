---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lamatic-openapi-generated.yml
  format: yaml
  label: Lamatic API
  slug: lamatic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lamatic/openapi/_ae-authored/lamatic-openapi-generated.yml
auth_types: []
description: Lamatic uses API keys for authentication. The API key is sent in the Authorization header using the Bearer token format.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Lamatic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lamatic declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Lamatic
provider_slug: lamatic
scheme_count: 2
schemes:
- evidence: 'Include your API key in the `Authorization` header of all GraphQL requests using the Bearer token format:'
  header: Authorization
  how_to_obtain: Create a new API key in Lamatic Studio → Settings → API Keys and copy the key.
  location: header
  name: Project API Key
  type: apiKey
- evidence: The Enterprise (org-level) API key (`lt-org-...`) is used for managing your Lamatic organization via the Enterprise API.
  header: Authorization
  how_to_obtain: Obtain from the Enterprise plan; see Lamatic documentation for details.
  location: header
  name: Enterprise API Key
  type: apiKey
slug: lamatic-authentication
source_filename: lamatic-authentication.yml
source_heading: Authentication Profile
source_url: https://lamatic.ai/docs/studio/studio-keys.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://lamatic.ai/docs/studio/studio-keys.md\nsources:\n- https://lamatic.ai/docs/studio/studio-keys.md\n- https://lamatic.ai/docs/api-integration/api-key.md\n- https://lamatic.ai/docs/api-integration/api-key\ndescription: Lamatic uses API keys for authentication. The API key is sent in the Authorization header using the Bearer token format.\nschemes:\n- type: apiKey\n  name: Project API Key\n  evidence: 'Include your API key in the `Authorization` header of all GraphQL requests using the Bearer token format:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a new API key in Lamatic Studio → Settings → API Keys and copy the key.\n- type: apiKey\n  name: Enterprise API Key\n  evidence: The Enterprise (org-level) API key (`lt-org-...`) is used for managing your Lamatic organization via the Enterprise API.\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Obtain from the Enterprise plan; see Lamatic documentation for details.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://lamatic.ai/docs/studio/studio-keys.md\n"
source_yaml_url: https://artifacts.apis.io/lamatic/authentication/lamatic-authentication.yml
summary_line: 2 schemes
tags:
- AI Middleware
- Generative AI
- Serverless deployment
- Integration
- Software-as-a-Service
- Enterprise
- Agency
---
