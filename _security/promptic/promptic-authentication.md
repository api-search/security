---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Promptic API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Promptic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Promptic declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Promptic
provider_slug: promptic
scheme_count: 2
schemes:
- evidence: 'Pass your API key as a Bearer token in the Authorization header:'
  header: Authorization
  how_to_obtain: Create API keys from the API Keys tab in an AI application's settings; the key value starts with "ptc_".
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'For browser-based integrations, use session cookies with the X-AI-Application-Id header:'
  header: Cookie
  how_to_obtain: Obtain a session cookie via browser login; include the cookie and the X-AI-Application-Id header in requests.
  location: header
  name: Session authentication
  type: other
slug: promptic-authentication
source_filename: promptic-authentication.yml
source_heading: Authentication Profile
source_url: https://promptic.eu/docs/guides/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://promptic.eu/docs/guides/authentication\nsources:\n- https://promptic.eu/docs/guides/authentication\n- https://promptic.eu/docs/openapi/ai-applications/get\n- https://promptic.eu/docs/guides/api-keys\n- https://promptic.eu/docs/guides/troubleshooting\ndescription: Authentication methods for Promptic API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Pass your API key as a Bearer token in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create API keys from the API Keys tab in an AI application's settings; the key value starts with \"ptc_\".\n- type: other\n  name: Session authentication\n  evidence: 'For browser-based integrations, use session cookies with the X-AI-Application-Id header:'\n  location: header\n  header: Cookie\n  how_to_obtain: Obtain a session cookie via browser login; include the cookie and the\
  \ X-AI-Application-Id header in requests.\ndocs: https://promptic.eu/docs/guides/authentication\n"
source_yaml_url: https://artifacts.apis.io/promptic/authentication/promptic-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Optimization
- Enterprise
- LLM
---
