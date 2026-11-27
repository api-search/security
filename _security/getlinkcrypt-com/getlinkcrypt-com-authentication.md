---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getlinkcrypt-com-openapi-generated.yml
  format: yaml
  label: Link Crypt API
  slug: getlinkcrypt-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getlinkcrypt-com/openapi/_ae-authored/getlinkcrypt-com-openapi-generated.yml
auth_types: []
description: Authentication methods published on Link Crypt pages
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Link Crypt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Link Crypt declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Link Crypt
provider_slug: getlinkcrypt-com
scheme_count: 2
schemes:
- evidence: 'API keys Use these keys with Authorization: Bearer … on the LinkCrypt REST API.'
  header: Authorization
  how_to_obtain: Create an API key in Preferences; the full secret is shown once.
  location: header
  name: API Key
  type: http-bearer
- evidence: choose OAuth for authentication, accept the warning, and create it.
  how_to_obtain: When adding a custom connector, select OAuth for authentication and approve the sign‑in.
  name: OAuth
  type: oauth2
slug: getlinkcrypt-com-authentication
source_filename: getlinkcrypt-com-authentication.yml
source_heading: Authentication Profile
source_url: https://getlinkcrypt.com/preferences
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getlinkcrypt.com/preferences\nsources:\n- https://getlinkcrypt.com/preferences\n- https://getlinkcrypt.com/onboarding\n- https://getlinkcrypt.com/integrations/mcp\ndescription: Authentication methods published on Link Crypt pages\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'API keys Use these keys with Authorization: Bearer … on the LinkCrypt REST API.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Preferences; the full secret is shown once.\n- type: oauth2\n  name: OAuth\n  evidence: choose OAuth for authentication, accept the warning, and create it.\n  how_to_obtain: When adding a custom connector, select OAuth for authentication and approve the sign‑in.\ndocs: https://getlinkcrypt.com/preferences\n"
source_yaml_url: https://artifacts.apis.io/getlinkcrypt-com/authentication/getlinkcrypt-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Bookmarking
- Knowledge Management
- Productivity
- LinkCrypt
---
