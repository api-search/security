---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for Mallory API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mallory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mallory declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Mallory
provider_slug: mallory
scheme_count: 1
schemes:
- evidence: Use API keys and Bearer tokens to authenticate with the Mallory API
  header: Authorization
  how_to_obtain: Generate an API key via the Mallory dashboard at https://app.mallory.ai/api/keys
  location: header
  name: Bearer
  type: http-bearer
slug: mallory-authentication
source_filename: mallory-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mallory.ai/build/api/auth.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mallory.ai/build/api/auth.md\nsources:\n- https://docs.mallory.ai/build/api/auth.md\n- https://docs.mallory.ai/use/auth/sso.md\n- https://docs.mallory.ai/use/auth/okta.md\n- https://docs.mallory.ai/use/auth/google.md\ndescription: Authentication schemes for Mallory API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Use API keys and Bearer tokens to authenticate with the Mallory API\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key via the Mallory dashboard at https://app.mallory.ai/api/keys\ndocs: https://docs.mallory.ai/build/api/auth.md\n"
source_yaml_url: https://artifacts.apis.io/mallory/authentication/mallory-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Threat Intelligence
- AI
- Platform
- Exposure Management
---
