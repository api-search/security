---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fettle-sh-api-openapi.json
  format: json
  label: fettle.sh Api API
  slug: fettle-sh-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fettle-sh/openapi/_original/fettle-sh-api-openapi.json
auth_types: []
description: Fettle uses API keys presented as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fettle Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: fettle-sh declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: fettle-sh
provider_slug: fettle-sh
scheme_count: 1
schemes:
- evidence: '-H "Authorization: Bearer fettle_your_key_here"'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys; the secret is shown once at creation.
  location: header
  name: Authorization
  type: http-bearer
slug: fettle-sh-authentication
source_filename: fettle-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://fettle.sh/docs/api-keys
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://fettle.sh/docs/api-keys\nsources:\n- https://fettle.sh/docs/api-keys\n- https://fettle.sh/docs/api-keys.md\n- https://fettle.sh/docs/quickstart\n- https://fettle.sh/docs/quickstart.md\ndescription: Fettle uses API keys presented as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: '-H \"Authorization: Bearer fettle_your_key_here\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys; the secret is shown once at creation.\nnote: No other authentication schemes (apiKey, oauth2, http-basic, jwt, hmac, mtls, other) are documented.\ndocs: https://fettle.sh/docs/api-keys\n"
source_yaml_url: https://artifacts.apis.io/fettle-sh/authentication/fettle-sh-authentication.yml
summary_line: 1 scheme
tags:
- Monitoring
- Uptime
- Developers
- AI Agents
- API
---
