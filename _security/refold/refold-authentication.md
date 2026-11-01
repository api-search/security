---
anonymous_access: false
api_key_in: []
api_specs:
- filename: refold-openapi-generated.yml
  format: yaml
  label: Refold API
  slug: refold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refold/openapi/_ae-authored/refold-openapi-generated.yml
auth_types: []
description: Authentication methods for Refold API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Refold Authentication
name_suffix: Authentication
oauth_flows: []
overview: Refold declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Refold
provider_slug: refold
scheme_count: 2
schemes:
- evidence: Organization API key, sent in the x-api-key header.
  header: x-api-key
  how_to_obtain: Generate an organization API key in the Refold dashboard; production keys start with pk, test keys with tk.
  location: header
  name: x-api-key
  type: apiKey
- evidence: The app must be an OAuth2 app.
  how_to_obtain: Configure OAuth client credentials (client ID, client secret, redirect URI) in the Refold app settings; then use the Get OAuth URL endpoint to obtain an authorization URL.
  name: OAuth2
  type: oauth2
slug: refold-authentication
source_filename: refold-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.refold.ai/api-reference/auth-structure/get-oauth-url
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.refold.ai/api-reference/auth-structure/get-oauth-url\nsources:\n- https://docs.refold.ai/api-reference/auth-structure/get-oauth-url\n- https://docs.refold.ai/applications/providers/netsuite_oauth\n- https://docs.refold.ai/resources/integration-providers/netsuite_oauth\n- https://docs.refold.ai/v3/api-reference/auth-structure/get-oauth-url\ndescription: Authentication methods for Refold API\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: Organization API key, sent in the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an organization API key in the Refold dashboard; production keys start with pk, test keys with tk.\n- type: oauth2\n  name: OAuth2\n  evidence: The app must be an OAuth2 app.\n  how_to_obtain: Configure OAuth client credentials (client ID, client secret, redirect URI) in the Refold app settings; then use the\
  \ Get OAuth\n    URL endpoint to obtain an authorization URL.\ndocs: https://docs.refold.ai/api-reference/auth-structure/get-oauth-url\n"
source_yaml_url: https://artifacts.apis.io/refold/authentication/refold-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Integration
- Enterprise
- Automation
---
