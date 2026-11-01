---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Ampersand API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ampersand Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ampersand declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ampersand
provider_slug: ampersand-ai
scheme_count: 2
schemes:
- evidence: 'All API endpoints require authenticated access via an API key passed as a header `X-Api-Key`: your Ampersand API key.'
  header: X-Api-Key
  how_to_obtain: Create API keys from the API Keys page in the Ampersand Dashboard.
  location: header
  name: X-Api-Key
  type: apiKey
- evidence: "security:\n  - APIKeyHeader: []\n  - Bearer: []"
  header: Authorization
  how_to_obtain: Obtain a JWT token as described in the Ampersand JWT authentication documentation.
  location: header
  name: Bearer
  type: http-bearer
slug: ampersand-ai-authentication
source_filename: ampersand-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ampersand.ai/api/key-auth.md
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ampersand.ai/api/key-auth.md\nsources:\n- https://docs.ampersand.ai/api/key-auth.md\n- https://docs.ampersand.ai/reference/oauth/generate-oauth-authorization-url.md\n- https://docs.ampersand.ai/reference/oauth/generate-oauth-authorization-url-for-existing-connection.md\n- https://docs.ampersand.ai/reference/oauth/generate-oauth-authorization-url\ndescription: Authentication methods for Ampersand API\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'All API endpoints require authenticated access via an API key passed as a header `X-Api-Key`: your Ampersand API key.'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create API keys from the API Keys page in the Ampersand Dashboard.\n- type: http-bearer\n  name: Bearer\n  evidence: \"security:\\n  - APIKeyHeader: []\\n  - Bearer: []\"\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain\
  \ a JWT token as described in the Ampersand JWT authentication documentation.\ndocs: https://docs.ampersand.ai/api/key-auth.md\n"
source_yaml_url: https://artifacts.apis.io/ampersand-ai/authentication/ampersand-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Integration
- Enterprise
- API
- Automation
---
